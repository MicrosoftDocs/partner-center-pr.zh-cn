---
title: 自定义设备的开箱体验与 Windows Autopilot 配置文件 |合作伙伴中心
description: 预配置设备的开箱体验使用 Autopilot 配置文件。
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot、 windows autopilot、 microsoft autopilot、 零接触部署、 oobe、 登录屏幕、 开箱
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162217"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="d5138-104">自定义设备的开箱体验与 Windows Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="d5138-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="d5138-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="d5138-105">**Applies to**</span></span>

- <span data-ttu-id="d5138-106">CSP 直接帐单合作伙伴、 间接提供商和间接经销商</span><span class="sxs-lookup"><span data-stu-id="d5138-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="d5138-107">如果您管理客户的设备，你可能需要自定义客户的用户的开箱体验 (OOBE)。</span><span class="sxs-lookup"><span data-stu-id="d5138-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="d5138-108">可以将新设备使用 Windows Autopilot 配置文件预配置设备交付给客户之前，并将新的配置文件应用到客户已购买的设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="d5138-109">此文章介绍了如何创建并应用到合作伙伴中心中的设备的 Autopilot 配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="d5138-110">如果您是不熟悉 Autopilot，查看以下文章中的信息：</span><span class="sxs-lookup"><span data-stu-id="d5138-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="d5138-111">Windows Autopilot 概述</span><span class="sxs-lookup"><span data-stu-id="d5138-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="d5138-112">Autopilot 部署参考指南</span><span class="sxs-lookup"><span data-stu-id="d5138-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="d5138-113">概述</span><span class="sxs-lookup"><span data-stu-id="d5138-113">Overview</span></span>

<span data-ttu-id="d5138-114">使用合作伙伴中心中的 Windows Autopilot 功能，可以创建自定义配置文件，以适用于客户的设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="d5138-115">在本文发布的时，以下配置文件设置已可用：</span><span class="sxs-lookup"><span data-stu-id="d5138-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="d5138-116">跳过的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="d5138-116">Skip privacy settings.</span></span> <span data-ttu-id="d5138-117">此可选的 Autopilot 配置文件设置使组织能够在 OOBE 过程不询问有关隐私设置。</span><span class="sxs-lookup"><span data-stu-id="d5138-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="d5138-118">禁用设备上创建的本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="d5138-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="d5138-119">组织可以决定是否过程完成后，设置设备的用户应具有管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="d5138-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="d5138-120">自动设置为工作或学校帐户的设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="d5138-121">Autopilot 注册的所有设备将自动被视为工作或学校的设备，因此不会在 OOBE 过程要求这一问题。</span><span class="sxs-lookup"><span data-stu-id="d5138-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="d5138-122">跳过 Cortana、 OneDrive 和 OEM 注册设置页。</span><span class="sxs-lookup"><span data-stu-id="d5138-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="d5138-123">Autopilot 注册的所有设备将在开箱体验 (OOBE) 过程中自动跳都过这些页。</span><span class="sxs-lookup"><span data-stu-id="d5138-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="d5138-124">跳过最终用户许可协议 (EULA)。</span><span class="sxs-lookup"><span data-stu-id="d5138-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="d5138-125">从 Windows 10 1709年版开始，组织可以决定跳过的 OOBE 过程显示 EULA 页面。</span><span class="sxs-lookup"><span data-stu-id="d5138-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="d5138-126">请参阅[Windows Autopilot EULA 上诉](#windows-autopilot-eula-dismissal)下面有关在 Windows 过程中跳过 EULA 页面考虑的重要信息设置。</span><span class="sxs-lookup"><span data-stu-id="d5138-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="d5138-127">以下配置文件和设备管理权限和限制适用：</span><span class="sxs-lookup"><span data-stu-id="d5138-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="d5138-128">CSP 合作伙伴可以继续为现有的客户必须与其分销商关系管理 Autopilot 配置文件，即使客户已删除的合作伙伴委派的管理权限。</span><span class="sxs-lookup"><span data-stu-id="d5138-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="d5138-129">为已添加的客户，可以管理现有的设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="d5138-130">不能管理你的客户已上传到 Microsoft Store for Business 或 Microsoft Intune 门户的设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="d5138-131">创建和管理合作伙伴中心中的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="d5138-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="d5138-132">在合作伙伴中心，可以创建 Windows Autopilot 部署配置文件并将其应用到设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="d5138-133">仅管理代理可以创建并应用配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="d5138-134">创建新的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="d5138-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="d5138-135">选择**客户**从合作伙伴中心菜单，然后选择客户要创建的 Autopilot 配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="d5138-136">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="d5138-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d5138-137">下**Windows Autopilot 配置文件**选择**添加新的配置文件**。</span><span class="sxs-lookup"><span data-stu-id="d5138-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="d5138-138">输入配置文件的名称和描述，然后配置 OOBE 设置。</span><span class="sxs-lookup"><span data-stu-id="d5138-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="d5138-139">从选择：</span><span class="sxs-lookup"><span data-stu-id="d5138-139">Choose from:</span></span>  

   - <span data-ttu-id="d5138-140">跳过安装程序中的隐私设置</span><span class="sxs-lookup"><span data-stu-id="d5138-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="d5138-141">在设置中禁用本地管理员帐户</span><span class="sxs-lookup"><span data-stu-id="d5138-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="d5138-142">在设置中自动跳过页面</span><span class="sxs-lookup"><span data-stu-id="d5138-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="d5138-143">(包括*自动选择安装程序的工作或学校*并*跳过 Cortana、 OneDrive 和 OEM 注册设置页*)</span><span class="sxs-lookup"><span data-stu-id="d5138-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="d5138-144">跳过最终用户许可协议 (EULA)</span><span class="sxs-lookup"><span data-stu-id="d5138-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="d5138-145">请参阅[Windows Autopilot EULA 上诉](#windows-autopilot-eula-dismissal)下面有关在 Windows 过程中跳过 EULA 页面考虑的重要信息设置。</span><span class="sxs-lookup"><span data-stu-id="d5138-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="d5138-146">完成后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="d5138-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="d5138-147">适用于客户的设备的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="d5138-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="d5138-148">下面的说明假定你已添加的客户的设备到合作伙伴中心，并且可以访问其设备列表。</span><span class="sxs-lookup"><span data-stu-id="d5138-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="d5138-149">如果你尚未添加客户的设备，请按照中的说明[将设备添加到客户的帐户](#add-devices-to-a-customers-account)然后按照以下步骤进行操作。</span><span class="sxs-lookup"><span data-stu-id="d5138-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="d5138-150">为客户创建 Autopilot 配置文件后，可以将其应用到客户的设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="d5138-151">选择**客户**从合作伙伴中心菜单，然后选择你创建客户的 Autopilot 配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="d5138-152">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="d5138-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d5138-153">下**适用于设备的配置文件**选择设备或设备组你想要添加到配置文件，然后选择**配置文件应用**。</span><span class="sxs-lookup"><span data-stu-id="d5138-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="d5138-154">您刚刚应用的配置文件中将出现**配置文件**列。</span><span class="sxs-lookup"><span data-stu-id="d5138-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="d5138-155">请按照以下步骤来验证该配置文件将会成功应用到设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="d5138-156">a.</span><span class="sxs-lookup"><span data-stu-id="d5138-156">a.</span></span>  <span data-ttu-id="d5138-157">将设备连接到网络并将其打开。</span><span class="sxs-lookup"><span data-stu-id="d5138-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="d5138-158">b.</span><span class="sxs-lookup"><span data-stu-id="d5138-158">b.</span></span>  <span data-ttu-id="d5138-159">验证是否显示相应的 OOBE 屏幕（如果有）。</span><span class="sxs-lookup"><span data-stu-id="d5138-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="d5138-160">c.</span><span class="sxs-lookup"><span data-stu-id="d5138-160">c.</span></span>  <span data-ttu-id="d5138-161">当 OOBE 进程停止时，设备重置为出厂默认设置来准备新的用户。</span><span class="sxs-lookup"><span data-stu-id="d5138-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="d5138-162">从客户的设备中删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="d5138-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="d5138-163">选择**客户**从合作伙伴中心菜单，然后选择你创建客户的 Autopilot 配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="d5138-164">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="d5138-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d5138-165">下**适用于设备的配置文件**选择你想要删除的配置文件，然后选择的设备**删除配置文件**。</span><span class="sxs-lookup"><span data-stu-id="d5138-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="d5138-166">删除设备中的配置文件不会从列表中删除该配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="d5138-167">如果你想要删除配置文件，请按照中的说明[更新或删除 Autopilot 配置文件](#update-or-delete-an-autopilot-profile)。</span><span class="sxs-lookup"><span data-stu-id="d5138-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="d5138-168">更新或删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="d5138-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="d5138-169">如果客户想要更改的开箱体验已寄给他们的设备后，可以更改合作伙伴中心中的配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="d5138-170">当客户的设备连接到 internet 时，它将在 OOBE 过程中下载最新的配置文件版本。</span><span class="sxs-lookup"><span data-stu-id="d5138-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="d5138-171">此外，任何时间客户将设备还原为其出厂默认设置，设备将再次下载最新的配置文件版本 OOBE 过程。</span><span class="sxs-lookup"><span data-stu-id="d5138-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="d5138-172">选择**客户**从合作伙伴中心菜单，然后选择您需要更改 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="d5138-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="d5138-173">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="d5138-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d5138-174">下**Windows Autopilot 配置文件**选择需要更新的配置文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="d5138-175">进行必要的更改，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="d5138-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="d5138-176">若要删除此配置文件，请选择**删除配置文件**从页面的右上角。</span><span class="sxs-lookup"><span data-stu-id="d5138-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="d5138-177">将设备添加到客户的帐户</span><span class="sxs-lookup"><span data-stu-id="d5138-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="d5138-178">销售代理和管理代理可以将设备添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="d5138-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="d5138-179">可以将自定义 Autopilot 配置文件应用于客户的设备之前，您必须能够访问客户的设备列表。</span><span class="sxs-lookup"><span data-stu-id="d5138-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="d5138-180">如果你打算使用 OEM 名称、 序列号和型号组合，请注意这些限制：</span><span class="sxs-lookup"><span data-stu-id="d5138-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="d5138-181">此元组仅适用于较新的设备 （4 k 哈希值，例如），不支持 128b 哈希 （RS2 和以前的设备）。</span><span class="sxs-lookup"><span data-stu-id="d5138-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="d5138-182">元组注册是区分大小写，因此文件中的数据必须与匹配的型号和制造商名称***完全***由 OEM 提供程序 （硬件提供程序） 提供。</span><span class="sxs-lookup"><span data-stu-id="d5138-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="d5138-183">请按照以下说明将设备添加到合作伙伴中心中的客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="d5138-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="d5138-184">选择**客户**从合作伙伴中心菜单，然后选择客户想要管理其设备。</span><span class="sxs-lookup"><span data-stu-id="d5138-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="d5138-185">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="d5138-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="d5138-186">下**适用于设备的配置文件**选择**添加设备**。</span><span class="sxs-lookup"><span data-stu-id="d5138-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="d5138-187">输入设备列表的名称，然后选择**浏览**将上载到合作伙伴中心 （在.csv 文件格式） 的客户的列表。</span><span class="sxs-lookup"><span data-stu-id="d5138-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="d5138-188">你应与你的设备购买收到此.csv 文件。</span><span class="sxs-lookup"><span data-stu-id="d5138-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="d5138-189">如果未收到的.csv 文件，则可以按照中的步骤创建一个自己[将设备添加到 Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)。</span><span class="sxs-lookup"><span data-stu-id="d5138-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="d5138-190">上传.csv 文件，然后选择**保存**。</span><span class="sxs-lookup"><span data-stu-id="d5138-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="d5138-191">如果尝试上传.csv 文件时遇到一条错误消息，检查文件的格式。</span><span class="sxs-lookup"><span data-stu-id="d5138-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="d5138-192">可以使用硬件哈希，或 OEM 名称、 序列号和模型 （在此列顺序） 或 Windows 产品 id。</span><span class="sxs-lookup"><span data-stu-id="d5138-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="d5138-193">此外可以使用旁边的链接中提供的示例.csv 文件**将设备添加**若要创建的设备列表。</span><span class="sxs-lookup"><span data-stu-id="d5138-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="d5138-194">Windows Autopilot EULA 上诉</span><span class="sxs-lookup"><span data-stu-id="d5138-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="d5138-195">重要信息</span><span class="sxs-lookup"><span data-stu-id="d5138-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="d5138-196">Windows Autopilot 可以为客户管理的设备上配置 Windows 的自定义的安装。</span><span class="sxs-lookup"><span data-stu-id="d5138-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="d5138-197">如果被授权执行此操作由客户，可以禁止显示或隐藏某些设置 Windows，包括 EULA （最终用户许可协议） 接受屏幕时正常呈现给用户的设置屏幕。</span><span class="sxs-lookup"><span data-stu-id="d5138-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="d5138-198">使用此函数，即表示你同意，禁止显示或隐藏旨在向用户提供通知或已从你的客户代表的隐藏条款，并且您，获取足够的许可和授权条款意味着接受任何屏幕客户 （无论组织或单个用户以这种情况可能），同意任何通知，并接受任何条款适用于你的客户。</span><span class="sxs-lookup"><span data-stu-id="d5138-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="d5138-199">这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。</span><span class="sxs-lookup"><span data-stu-id="d5138-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="d5138-200">如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。</span><span class="sxs-lookup"><span data-stu-id="d5138-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>