---
title: 管理客户帐户的用户
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 管理客户在 合作伙伴中心 - 创建用户帐户、添加或删除用户许可证、重置密码以及删除或还原用户帐户。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149887"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="5ce90-103">管理客户帐户的用户和用户许可证</span><span class="sxs-lookup"><span data-stu-id="5ce90-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="5ce90-104">**适当的角色**：全局管理员|用户管理管理员|管理员代理</span><span class="sxs-lookup"><span data-stu-id="5ce90-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="5ce90-105">可以在客户的帐户中创建和删除新用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="5ce90-106">还可以还原在删除后 30 天内删除的一个或多个用户帐户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="5ce90-107">用户之前分配的订阅也将还原（假设之前的分配可用）。</span><span class="sxs-lookup"><span data-stu-id="5ce90-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="5ce90-108">为客户购买新订阅时，客户应提供需要帐户、用户权限以及每个用户所需服务的所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="5ce90-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="5ce90-109">"**客户"** 选项卡的"用户和许可证"部分显示特定客户租户中创建的所有用户，包括拥有从其他 CSP 合作伙伴或其他购买渠道购买的许可证的用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="5ce90-110">可以一次[将订阅分配给多个用户](bulk-license-provisioning-for-multiple-users.md)，方法是使用 [Excel 兼容的 .csv 电子表格文件](adding-multiple-users-to-a-customer-account.md)导入这些名称。</span><span class="sxs-lookup"><span data-stu-id="5ce90-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="5ce90-111">为客户创建用户帐户</span><span class="sxs-lookup"><span data-stu-id="5ce90-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="5ce90-112">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="5ce90-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5ce90-113">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="5ce90-114">在客户菜单中，选择"**用户和许可证"。**</span><span class="sxs-lookup"><span data-stu-id="5ce90-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="5ce90-115">对于每个用户，请选择 **添加订阅**，然后填写信息，包括权限和许可证。</span><span class="sxs-lookup"><span data-stu-id="5ce90-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="5ce90-116">单击“保存”以保存更改。</span><span class="sxs-lookup"><span data-stu-id="5ce90-116">**Save** your changes.</span></span>

5. <span data-ttu-id="5ce90-117">请确保记录用户名和临时密码以发送给用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="5ce90-118">如果要一次一个地添加多个用户，则使用 **再次添加一个用户**。</span><span class="sxs-lookup"><span data-stu-id="5ce90-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="5ce90-119">你还可以通过[导入 Excel 兼容的 .csv 电子表格文件](adding-multiple-users-to-a-customer-account.md)一次添加多个用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="5ce90-120">等到添加完所有用户后，可从确认屏幕通过电子邮件发送或打印这些名称和密码。</span><span class="sxs-lookup"><span data-stu-id="5ce90-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="5ce90-121">为客户添加或删除用户许可证</span><span class="sxs-lookup"><span data-stu-id="5ce90-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="5ce90-122">以下步骤适用于添加或删除 Microsoft 产品的用户许可证。</span><span class="sxs-lookup"><span data-stu-id="5ce90-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="5ce90-123">若要在商业市场中为基于许可证的 SaaS 订阅添加或删除用户许可证，请参阅添加或删除 [SaaS 订阅的许可证](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)。</span><span class="sxs-lookup"><span data-stu-id="5ce90-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="5ce90-124">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="5ce90-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5ce90-125">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="5ce90-126">在客户菜单中，选择"**用户和许可证"。**</span><span class="sxs-lookup"><span data-stu-id="5ce90-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="5ce90-127">从列表中选择一个或多个用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-127">Choose one or more users from the list.</span></span> <span data-ttu-id="5ce90-128">例如，如果客户刚刚购买了新许可证，而你想要将其分配给还没有许可证的用户，可以使用"按 **...** 筛选用户"选项来查找正确的组。</span><span class="sxs-lookup"><span data-stu-id="5ce90-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="5ce90-129">选择“管理许可证”。</span><span class="sxs-lookup"><span data-stu-id="5ce90-129">Select **Manage licenses**.</span></span> <span data-ttu-id="5ce90-130">进行更改 **，然后保存**。</span><span class="sxs-lookup"><span data-stu-id="5ce90-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="5ce90-131">对于 [Azure 市场，](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)许可证分配和激活通过发布产品的独立软件供应商 (ISV) 进行管理。</span><span class="sxs-lookup"><span data-stu-id="5ce90-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="5ce90-132">为客户重置用户密码</span><span class="sxs-lookup"><span data-stu-id="5ce90-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="5ce90-133">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="5ce90-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="5ce90-134">在“合作伙伴中心”菜单中，选择“客户”，然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="5ce90-135">在客户菜单中，选择"**用户和许可证"。**</span><span class="sxs-lookup"><span data-stu-id="5ce90-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="5ce90-136">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="5ce90-137">在屏幕底部，选择"重置 **密码"。**</span><span class="sxs-lookup"><span data-stu-id="5ce90-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="5ce90-138">将新的临时密码发送给用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="5ce90-139">为客户删除用户帐户</span><span class="sxs-lookup"><span data-stu-id="5ce90-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="5ce90-140">从 **"合作伙伴中心** 菜单中，选择"客户 **"。**</span><span class="sxs-lookup"><span data-stu-id="5ce90-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="5ce90-141">从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="5ce90-142">在客户菜单中，选择"**用户和许可证"。**</span><span class="sxs-lookup"><span data-stu-id="5ce90-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="5ce90-143">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="5ce90-144">在屏幕底部选择“删除用户帐户”。</span><span class="sxs-lookup"><span data-stu-id="5ce90-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="5ce90-145">如果需要还原此帐户，可在客户的 **用户和许可证** 列表的 **已删除用户** 选项卡中找到它。</span><span class="sxs-lookup"><span data-stu-id="5ce90-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="5ce90-146">你有 30 天的时间还原已删除的用户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="5ce90-147">还原删除的用户帐户</span><span class="sxs-lookup"><span data-stu-id="5ce90-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="5ce90-148">从合作伙伴中心 **菜单中** ，选择" **客户"，** 然后从列表中选择客户。</span><span class="sxs-lookup"><span data-stu-id="5ce90-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="5ce90-149">选择 " **用户和许可证**"。</span><span class="sxs-lookup"><span data-stu-id="5ce90-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="5ce90-150">选择 **已删除的用户 ( )**，当存在可以还原的已删除用户时，应读取 **(1)** 或更大。</span><span class="sxs-lookup"><span data-stu-id="5ce90-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="5ce90-151">选择一个或多个已删除用户的复选框，然后选择 " **还原**"。</span><span class="sxs-lookup"><span data-stu-id="5ce90-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="5ce90-152">所有选定的用户帐户将重新出现在 " **用户和许可证** " 页中。</span><span class="sxs-lookup"><span data-stu-id="5ce90-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5ce90-153">后续步骤</span><span class="sxs-lookup"><span data-stu-id="5ce90-153">Next steps</span></span>

- [<span data-ttu-id="5ce90-154">向多个用户分配或撤消许可证</span><span class="sxs-lookup"><span data-stu-id="5ce90-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="5ce90-155">为客户帐户创建多个用户</span><span class="sxs-lookup"><span data-stu-id="5ce90-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)