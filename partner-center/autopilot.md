---
title: 自定义设备全新体验
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 提供客户的新设备之前，可以使用 Windows Autopilot 配置文件自定义或预先配置设备的全新体验（OOBE）。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a59b0c25b8f5203942e73b549d5ffb9d65d90c36
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527653"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="2b8fa-103">使用新设备上的 Windows Autopilot 配置文件自定义客户全新体验</span><span class="sxs-lookup"><span data-stu-id="2b8fa-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="2b8fa-104">**适用于**</span><span class="sxs-lookup"><span data-stu-id="2b8fa-104">**Applies to**</span></span>

- <span data-ttu-id="2b8fa-105">CSP 直接帐单合作伙伴、间接提供商和间接经销商</span><span class="sxs-lookup"><span data-stu-id="2b8fa-105">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="2b8fa-106">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="2b8fa-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2b8fa-107">管理员代理</span><span class="sxs-lookup"><span data-stu-id="2b8fa-107">Admin agent</span></span>
- <span data-ttu-id="2b8fa-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="2b8fa-108">Global admin</span></span>
- <span data-ttu-id="2b8fa-109">销售代理</span><span class="sxs-lookup"><span data-stu-id="2b8fa-109">Sales agent</span></span>
- <span data-ttu-id="2b8fa-110">“用户管理”管理员</span><span class="sxs-lookup"><span data-stu-id="2b8fa-110">User management admin</span></span>

<span data-ttu-id="2b8fa-111">如果你管理客户设备，你可能需要为客户的用户自定义全新体验（OOBE）。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-111">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="2b8fa-112">在将设备交付给客户并将新的配置文件应用于客户已购买的设备之前，可以使用 Windows Autopilot 配置文件预先配置新设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-112">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="2b8fa-113">请注意，Oem 已开始在显示设备的**产品密钥 ID （PKID）** 的 Autopilot 设备框之外添加发货标签。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-113">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="2b8fa-114">这一维的可读条形码为下游合作伙伴提供了一种方法，用于为 Autopilot 注册设备，无需取消装箱设备并通过替代方法获取设备 ID。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-114">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="2b8fa-115">本文介绍如何创建 Autopilot 配置文件并将其应用于合作伙伴中心的设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-115">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="2b8fa-116">如果你尚不熟悉 Autopilot，请查看以下文章中的信息：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-116">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="2b8fa-117">Windows Autopilot 概述</span><span class="sxs-lookup"><span data-stu-id="2b8fa-117">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="2b8fa-118">Autopilot 部署参考指南</span><span class="sxs-lookup"><span data-stu-id="2b8fa-118">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="2b8fa-119">概述</span><span class="sxs-lookup"><span data-stu-id="2b8fa-119">Overview</span></span>

<span data-ttu-id="2b8fa-120">使用合作伙伴中心的 Windows Autopilot 功能，你可以创建自定义配置文件以应用于客户设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-120">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="2b8fa-121">以下配置文件设置在本文发布时可用：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-121">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="2b8fa-122">跳过隐私设置。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-122">Skip privacy settings.</span></span> <span data-ttu-id="2b8fa-123">此可选的 Autopilot 配置文件设置使组织无在 OOBE 过程中询问隐私设置。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-123">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="2b8fa-124">禁用设备上的本地管理员帐户创建。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-124">Disable local admin account creation on the device.</span></span> <span data-ttu-id="2b8fa-125">组织可决定在完成该过程后，设置设备的用户是否应具有管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-125">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="2b8fa-126">为工作或学校自动设置设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-126">Automatically set up device for work or school.</span></span> <span data-ttu-id="2b8fa-127">注册到 Autopilot 的所有设备将自动被视为工作或学校设备，因此不会在 OOBE 过程中询问此问题。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-127">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="2b8fa-128">跳过 Cortana、OneDrive 和 OEM 注册设置页。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-128">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="2b8fa-129">注册到 Autopilot 的所有设备都会在全新体验（OOBE）过程中自动跳过这些页面。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-129">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="2b8fa-130">跳过最终用户许可协议（EULA）。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-130">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="2b8fa-131">从 Windows 10 版本1709开始，组织可以决定跳过 OOBE 过程中显示的 EULA 页面。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-131">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="2b8fa-132">请参阅下面的[Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal)，以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-132">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="2b8fa-133">以下配置文件和设备管理权限和限制适用：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-133">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="2b8fa-134">即使客户已删除合作伙伴的委派管理权限，CSP 合作伙伴也可以继续管理与其拥有分销商关系的现有客户的 Autopilot 配置文件。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-134">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="2b8fa-135">你可以管理已添加的客户的现有设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-135">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="2b8fa-136">你无法管理客户已上传到 Microsoft Store for Business 或 Microsoft Intune 门户的设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-136">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="2b8fa-137">在合作伙伴中心创建和管理 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="2b8fa-137">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="2b8fa-138">在合作伙伴中心，你可以创建 Windows Autopilot 部署配置文件并将它们应用到设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-138">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="2b8fa-139">只有管理代理可以创建和应用配置文件。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-139">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="2b8fa-140">创建新的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="2b8fa-140">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="2b8fa-141">从 "合作伙伴中心" 菜单中选择 "**客户**"，然后选择要为其创建 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-141">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b8fa-142">在客户的详细信息页上，选择 "**设备**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-142">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b8fa-143">在 " **Windows Autopilot 配置文件**" 下，选择 "**添加新配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-143">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="2b8fa-144">输入配置文件的 "名称" 和 "说明"，然后配置 "OOBE" 设置。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-144">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="2b8fa-145">选择：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-145">Choose from:</span></span>  

   - <span data-ttu-id="2b8fa-146">在安装程序中跳过隐私设置</span><span class="sxs-lookup"><span data-stu-id="2b8fa-146">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="2b8fa-147">在设置中禁用本地管理员帐户</span><span class="sxs-lookup"><span data-stu-id="2b8fa-147">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="2b8fa-148">在设置中自动跳过页面</span><span class="sxs-lookup"><span data-stu-id="2b8fa-148">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="2b8fa-149">（包括*自动选择适用于工作或学校的设置*，并*跳过 Cortana、OneDrive 和 OEM 注册设置页*）</span><span class="sxs-lookup"><span data-stu-id="2b8fa-149">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="2b8fa-150">跳过最终用户许可协议（EULA）</span><span class="sxs-lookup"><span data-stu-id="2b8fa-150">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="2b8fa-151">请参阅下面的[Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal)，以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-151">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="2b8fa-152">完成后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-152">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="2b8fa-153">将 Autopilot 配置文件应用到客户设备</span><span class="sxs-lookup"><span data-stu-id="2b8fa-153">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="2b8fa-154">以下说明假定您已将客户的设备添加到合作伙伴中心，并且您可以访问其设备列表。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-154">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="2b8fa-155">如果尚未添加客户的设备，请按照[将设备添加到客户帐户](#add-devices-to-a-customers-account)中的说明操作，然后执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-155">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="2b8fa-156">为客户创建 Autopilot 配置文件后，可将其应用到客户的设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-156">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="2b8fa-157">从 "合作伙伴中心" 菜单中选择 "**客户**"，然后选择为其创建 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-157">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b8fa-158">在客户的详细信息页上，选择 "**设备**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-158">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b8fa-159">在 "**将配置文件应用到设备**" 下，选择要将配置文件添加到的设备或设备组，然后选择 "**应用配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-159">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="2b8fa-160">刚才应用的配置文件将显示在 "**配置文件**" 列中。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-160">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="2b8fa-161">按照以下步骤验证配置文件是否将成功应用到设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-161">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="2b8fa-162">a.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-162">a.</span></span>  <span data-ttu-id="2b8fa-163">将设备连接到网络并将其打开。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-163">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="2b8fa-164">b.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-164">b.</span></span>  <span data-ttu-id="2b8fa-165">验证是否显示相应的 OOBE 屏幕（如果有）。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-165">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="2b8fa-166">c.</span><span class="sxs-lookup"><span data-stu-id="2b8fa-166">c.</span></span>  <span data-ttu-id="2b8fa-167">当 OOBE 进程停止时，将设备重置为其出厂默认设置，以便为新用户准备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-167">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="2b8fa-168">从客户的设备中删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="2b8fa-168">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="2b8fa-169">从 "合作伙伴中心" 菜单中选择 "**客户**"，然后选择为其创建 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-169">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b8fa-170">在客户的详细信息页上，选择 "**设备**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-170">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b8fa-171">在 "**将配置文件应用到设备**" 下，选择要从中删除配置文件的设备，然后选择 "**删除配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-171">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="2b8fa-172">从设备删除配置文件不会从列表中删除该配置文件。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-172">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="2b8fa-173">如果要删除配置文件，请按照[更新或删除 Autopilot 配置文件](#update-or-delete-an-autopilot-profile)中的说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-173">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="2b8fa-174">更新或删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="2b8fa-174">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="2b8fa-175">如果客户想要在将设备寄送到设备后更改全新体验，可以在合作伙伴中心更改该配置文件。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-175">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="2b8fa-176">当客户的设备连接到 internet 时，它将在 OOBE 过程中下载最新的配置文件版本。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-176">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="2b8fa-177">此外，在任何时候，如果客户将设备恢复为其出厂默认设置，则设备将在 OOBE 过程中再次下载最新的配置文件版本。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-177">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="2b8fa-178">从 "合作伙伴中心" 菜单中选择 "**客户**"，然后选择要更改 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-178">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="2b8fa-179">在客户的详细信息页上，选择 "**设备**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-179">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b8fa-180">在 " **Windows Autopilot 配置文件**" 下，选择需要更新的配置文件。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-180">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="2b8fa-181">进行所需的更改，然后选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-181">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="2b8fa-182">若要删除此配置文件，请选择页面右上角的 "**删除配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-182">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="2b8fa-183">向客户帐户添加设备</span><span class="sxs-lookup"><span data-stu-id="2b8fa-183">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="2b8fa-184">销售代理和管理代理可以将设备添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-184">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="2b8fa-185">你必须能够访问客户的设备列表，然后才能将自定义 Autopilot 配置文件应用到客户设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-185">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="2b8fa-186">如果计划使用 OEM 名称、序列号和型号组合，请注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-186">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="2b8fa-187">此元组仅适用于较新的设备（例如4k 哈希），不支持128b 哈希（RS2 和之前的设备）。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-187">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="2b8fa-188">元组注册区分大小写，因此文件中的数据必须与 OEM 提供商（硬件提供商）提供的名称***完全***匹配。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-188">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="2b8fa-189">按照以下说明将设备添加到合作伙伴中心的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-189">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="2b8fa-190">从 "合作伙伴中心" 菜单中选择 "**客户**"，然后选择要管理其设备的客户。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-190">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="2b8fa-191">在客户的详细信息页上，选择 "**设备**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-191">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b8fa-192">在 "**将配置文件应用到设备**" 下选择 "**添加设备**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-192">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="2b8fa-193">输入 "设备列表" 的名称，然后选择 "**浏览**" 以将客户列表（采用 .csv 文件格式）上传到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-193">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2b8fa-194">你应收到此 .csv 文件，并购买你的设备。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-194">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="2b8fa-195">如果未收到 .csv 文件，则可以按照[向 Windows Autopilot 中添加设备](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步骤自行创建。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-195">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="2b8fa-196">上传 .csv 文件，然后选择 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-196">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="2b8fa-197">如果在尝试上传 .csv 文件时收到错误消息，请检查该文件的格式。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-197">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="2b8fa-198">您可以仅使用硬件哈希，或使用 OEM 名称、序列号和型号（列顺序）或 Windows 产品 ID。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-198">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="2b8fa-199">你还可以使用 "**添加设备**" 下的链接中提供的示例 .csv 文件来创建设备列表。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-199">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="2b8fa-200">.Csv 文件应如下所示：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-200">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="2b8fa-201">**设备序列号、Windows 产品 ID、硬件哈希、制造商名称、设备型号**</span><span class="sxs-lookup"><span data-stu-id="2b8fa-201">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="2b8fa-202">**{serialNumber},,, Microsoft Corporation，Surface 便携机**</span><span class="sxs-lookup"><span data-stu-id="2b8fa-202">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="2b8fa-203">"制造商名称" 和 "设备型号" 区分大小写。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-203">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="2b8fa-204">如果你不知道要为制造商名称和设备型号放入哪个值，则可以在设备上运行此值以收集正确的值：</span><span class="sxs-lookup"><span data-stu-id="2b8fa-204">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="2b8fa-205">Windows Autopilot EULA 消除</span><span class="sxs-lookup"><span data-stu-id="2b8fa-205">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="2b8fa-206">重要信息</span><span class="sxs-lookup"><span data-stu-id="2b8fa-206">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="2b8fa-207">Windows Autopilot 允许你在为客户管理的设备上配置 Windows 的自定义安装。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-207">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="2b8fa-208">如果客户有权执行此操作，则可以禁止或隐藏在设置 Windows 时通常向用户显示的某些安装屏幕，包括 EULA （最终用户许可协议）接受屏幕。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-208">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="2b8fa-209">通过使用此函数，你同意禁止或隐藏旨在向用户提供通知或接受条款的任何屏幕，这意味着你已获得了对你的客户的充分同意和授权，以隐藏条款，并且你代表你的客户（无论是组织还是单个用户作为案例），同意通知并接受适用于你的客户的任何条款。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-209">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="2b8fa-210">这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-210">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="2b8fa-211">如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。</span><span class="sxs-lookup"><span data-stu-id="2b8fa-211">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
