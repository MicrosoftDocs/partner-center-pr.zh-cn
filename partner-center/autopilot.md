---
title: 自定义设备的全新的全新体验的 Windows Autopilot 配置文件 |合作伙伴中心
description: 预配置的 Autopilot 配置文件的设备的现成的体验。
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: autopilot，windows autopilot、 microsoft autopilot，零接触部署，oobe，登录屏幕，现成的
ms.localizationpriority: medium
ms.openlocfilehash: d563ad09d1fa3b67b01835480a348a524455efbc
ms.sourcegitcommit: f1c269f4ac52d5206d65d9585855da309f0aae8a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2019
ms.locfileid: "9083400"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="87409-104">自定义设备的全新的全新体验的 Windows Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="87409-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="87409-105">适用范围</span><span class="sxs-lookup"><span data-stu-id="87409-105">Applies to</span></span>**

- <span data-ttu-id="87409-106">云解决方案提供商直接帐单合作伙伴，间接提供商和间接经销商</span><span class="sxs-lookup"><span data-stu-id="87409-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="87409-107">如果你管理客户的设备，你可能需要自定义的全新体验 (OOBE) 的客户的用户。</span><span class="sxs-lookup"><span data-stu-id="87409-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="87409-108">你可以预交付给客户的设备之前配置的 Windows Autopilot 配置文件的新设备，并将新的配置文件应用到客户已购买的设备。</span><span class="sxs-lookup"><span data-stu-id="87409-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="87409-109">本文介绍了如何创建 Autopilot 配置文件并应用到合作伙伴中心中的设备。</span><span class="sxs-lookup"><span data-stu-id="87409-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="87409-110">如果你还不熟悉使用 Autopilot，查看这些文章中的信息：</span><span class="sxs-lookup"><span data-stu-id="87409-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="87409-111">Windows Autopilot 概述</span><span class="sxs-lookup"><span data-stu-id="87409-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="87409-112">Autopilot 部署参考指南</span><span class="sxs-lookup"><span data-stu-id="87409-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="87409-113">概述</span><span class="sxs-lookup"><span data-stu-id="87409-113">Overview</span></span>

<span data-ttu-id="87409-114">与合作伙伴中心中的 Windows Autopilot 功能，你可以创建自定义配置文件将应用于客户设备。</span><span class="sxs-lookup"><span data-stu-id="87409-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="87409-115">在本文发表时，以下配置文件设置都不可用：</span><span class="sxs-lookup"><span data-stu-id="87409-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="87409-116">跳过隐私设置。</span><span class="sxs-lookup"><span data-stu-id="87409-116">Skip privacy settings.</span></span> <span data-ttu-id="87409-117">此可选的 Autopilot 配置文件设置可让组织在 OOBE 过程中不询问有关隐私设置。</span><span class="sxs-lookup"><span data-stu-id="87409-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="87409-118">禁用在设备上的创建本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="87409-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="87409-119">组织可以决定是否过程完成后，设置设备的用户应拥有管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="87409-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="87409-120">自动设置为工作单位或学校的设备。</span><span class="sxs-lookup"><span data-stu-id="87409-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="87409-121">使用 Autopilot 注册的所有设备自动将被视为工作或学校的设备，因此不会在 OOBE 过程中要求此问题。</span><span class="sxs-lookup"><span data-stu-id="87409-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="87409-122">跳过 Cortana、 OneDrive 和 OEM 注册设置页面。</span><span class="sxs-lookup"><span data-stu-id="87409-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="87409-123">使用 Autopilot 注册的所有设备将在外的全新体验 (OOBE) 过程中自动跳都过这些页面。</span><span class="sxs-lookup"><span data-stu-id="87409-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="87409-124">跳过最终用户许可协议 (EULA)。</span><span class="sxs-lookup"><span data-stu-id="87409-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="87409-125">从 Windows 10 版本 1709年开始，组织可以决定跳过 OOBE 过程中显示的最终用户许可协议页面。</span><span class="sxs-lookup"><span data-stu-id="87409-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="87409-126">请参阅[Windows Autopilot EULA 解除](#windows-autopilot-eula-dismissal)下面的重要信息需要考虑有关在 Windows 安装程序期间跳过 EULA 页。</span><span class="sxs-lookup"><span data-stu-id="87409-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="87409-127">以下配置文件和设备的管理权限和限制应用：</span><span class="sxs-lookup"><span data-stu-id="87409-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="87409-128">云解决方案提供商合作伙伴可以继续为与他们有经销商关系的现有客户管理 Autopilot 配置文件，即使客户已经删除合作伙伴的委派的管理权限。</span><span class="sxs-lookup"><span data-stu-id="87409-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="87409-129">你可以为你的或由另一个云解决方案提供商合作伙伴已添加的客户管理现有设备。</span><span class="sxs-lookup"><span data-stu-id="87409-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="87409-130">不能管理你的客户已上传到适用于企业的 Microsoft 应用商店或 Microsoft Intune 门户的设备。</span><span class="sxs-lookup"><span data-stu-id="87409-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="87409-131">创建和管理合作伙伴中心中的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="87409-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="87409-132">在合作伙伴中心中，你可以创建 Windows Autopilot 部署配置文件，并将它们应用到设备。</span><span class="sxs-lookup"><span data-stu-id="87409-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="87409-133">只有管理员代理可以创建并应用配置文件。</span><span class="sxs-lookup"><span data-stu-id="87409-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="87409-134">创建新的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="87409-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="87409-135">从合作伙伴中心菜单中选择**客户**，然后选择你要创建的 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="87409-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="87409-136">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="87409-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="87409-137">在**Windows Autopilot 配置文件**选择**添加新配置文件**。</span><span class="sxs-lookup"><span data-stu-id="87409-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="87409-138">输入配置文件的名称和描述，然后配置 OOBE 设置。</span><span class="sxs-lookup"><span data-stu-id="87409-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="87409-139">从选择：</span><span class="sxs-lookup"><span data-stu-id="87409-139">Choose from:</span></span>  

   - <span data-ttu-id="87409-140">在设置中跳过隐私设置</span><span class="sxs-lookup"><span data-stu-id="87409-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="87409-141">在设置中禁用本地管理员帐户</span><span class="sxs-lookup"><span data-stu-id="87409-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="87409-142">在设置中自动跳过页面</span><span class="sxs-lookup"><span data-stu-id="87409-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="87409-143">（包括*为工作单位或学校自动选择设置*和*跳过 Cortana、 OneDrive 和 OEM 注册设置页面*）</span><span class="sxs-lookup"><span data-stu-id="87409-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="87409-144">跳过最终用户许可协议 (EULA)</span><span class="sxs-lookup"><span data-stu-id="87409-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="87409-145">请参阅[Windows Autopilot EULA 解除](#windows-autopilot-eula-dismissal)下面的重要信息需要考虑有关在 Windows 安装程序期间跳过 EULA 页。</span><span class="sxs-lookup"><span data-stu-id="87409-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="87409-146">完成后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="87409-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="87409-147">适用于客户设备的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="87409-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="87409-148">以下说明假设，已经向合作伙伴中心添加客户的设备，并且可以访问其设备列表。</span><span class="sxs-lookup"><span data-stu-id="87409-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="87409-149">如果你尚未添加客户的设备，按照[客户的帐户添加设备](#add-devices-to-a-customers-account)中的说明，然后按照下面的步骤。</span><span class="sxs-lookup"><span data-stu-id="87409-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="87409-150">为客户创建 Autopilot 配置文件后，你可以将其应用到客户的设备。</span><span class="sxs-lookup"><span data-stu-id="87409-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="87409-151">从合作伙伴中心菜单中选择**客户**，然后选择你创建的 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="87409-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="87409-152">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="87409-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="87409-153">在**应用到设备的配置文件**选择设备或你想要添加到配置文件，然后选择**应用配置文件**的设备组。</span><span class="sxs-lookup"><span data-stu-id="87409-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="87409-154">只是应用的配置文件将显示在**配置文件**列中。</span><span class="sxs-lookup"><span data-stu-id="87409-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="87409-155">请按照以下步骤来验证配置文件将会成功应用到设备。</span><span class="sxs-lookup"><span data-stu-id="87409-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="87409-156">a.</span><span class="sxs-lookup"><span data-stu-id="87409-156">a.</span></span>  <span data-ttu-id="87409-157">将设备连接到网络，并将其打开。</span><span class="sxs-lookup"><span data-stu-id="87409-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="87409-158">b.</span><span class="sxs-lookup"><span data-stu-id="87409-158">b.</span></span>  <span data-ttu-id="87409-159">验证是否显示相应的 OOBE 屏幕（如果有）。</span><span class="sxs-lookup"><span data-stu-id="87409-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="87409-160">c.</span><span class="sxs-lookup"><span data-stu-id="87409-160">c.</span></span>  <span data-ttu-id="87409-161">当在 OOBE 过程停止时，设备重置为出厂默认设置为新用户准备。</span><span class="sxs-lookup"><span data-stu-id="87409-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="87409-162">从客户的设备中删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="87409-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="87409-163">从合作伙伴中心菜单中选择**客户**，然后选择你创建的 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="87409-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="87409-164">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="87409-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="87409-165">在**应用到设备的配置文件**中，选择你想要删除的配置文件，然后选择**删除配置文件**的设备。</span><span class="sxs-lookup"><span data-stu-id="87409-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="87409-166">从设备中删除配置文件不会从列表中删除配置文件。</span><span class="sxs-lookup"><span data-stu-id="87409-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="87409-167">如果你想要删除配置文件，请按照[更新或删除 Autopilot 配置文件](#update-or-delete-an-autopilot-profile)中的说明。</span><span class="sxs-lookup"><span data-stu-id="87409-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="87409-168">更新或删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="87409-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="87409-169">如果客户想要更改的全新体验后已交付给他们的设备，你可以更改合作伙伴中心中的配置文件。</span><span class="sxs-lookup"><span data-stu-id="87409-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="87409-170">当客户的设备连接到 internet 时，它将在 OOBE 过程中下载最新的配置文件版本。</span><span class="sxs-lookup"><span data-stu-id="87409-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="87409-171">此外，客户将设备还原为出厂默认设置，任何时间该设备将重新下载最新的配置文件版本在 OOBE 过程。</span><span class="sxs-lookup"><span data-stu-id="87409-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="87409-172">从合作伙伴中心菜单中选择**客户**，然后选择想要更改 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="87409-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="87409-173">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="87409-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="87409-174">在**Windows Autopilot 配置文件**中，选择你需要更新的配置文件。</span><span class="sxs-lookup"><span data-stu-id="87409-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="87409-175">执行所需的更改，然后选择**提交**。</span><span class="sxs-lookup"><span data-stu-id="87409-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="87409-176">若要删除此配置文件，选择从该页面的右上角的**删除配置文件**。</span><span class="sxs-lookup"><span data-stu-id="87409-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="87409-177">将设备添加到客户的帐户</span><span class="sxs-lookup"><span data-stu-id="87409-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="87409-178">销售代理和管理员代理可以将设备添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="87409-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="87409-179">你可以将自定义的 Autopilot 配置文件应用于客户设备之前，你必须能够访问客户的设备列表。</span><span class="sxs-lookup"><span data-stu-id="87409-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="87409-180">如果你计划使用 OEM 名称、 序列号和模型组合，应注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="87409-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="87409-181">此元组仅适用于的较新的设备 （4 个 k 哈希，例如） 并且 128b 哈希 （RS2 和之前的设备） 不受支持。</span><span class="sxs-lookup"><span data-stu-id="87409-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="87409-182">元组注册是区分大小写，因此文件中的数据必须型号和制造商的名称***完全***匹配，因为由 OEM 提供程序 （硬件提供程序） 提供。</span><span class="sxs-lookup"><span data-stu-id="87409-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="87409-183">请按照以下说明将设备添加到合作伙伴中心中的客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="87409-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="87409-184">从合作伙伴中心菜单中选择**客户**，然后选择客户想要管理其设备。</span><span class="sxs-lookup"><span data-stu-id="87409-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="87409-185">在客户的详细信息页上，选择**设备**。</span><span class="sxs-lookup"><span data-stu-id="87409-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="87409-186">在**应用到设备的配置文件**下选择**添加设备**。</span><span class="sxs-lookup"><span data-stu-id="87409-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="87409-187">输入设备列表的名称，然后选择**浏览**（在.csv 文件格式） 的客户的列表上传到合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="87409-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="87409-188">你应该使用设备购买收到此.csv 文件。</span><span class="sxs-lookup"><span data-stu-id="87409-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="87409-189">如果你未收到.csv 文件，你可以按照[添加 Windows Autopilot 设备](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步骤来创建自己。</span><span class="sxs-lookup"><span data-stu-id="87409-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="87409-190">上传.csv 文件，然后选择**保存**。</span><span class="sxs-lookup"><span data-stu-id="87409-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="87409-191">如果你尝试上传.csv 文件时收到一条错误消息，请检查文件的格式。</span><span class="sxs-lookup"><span data-stu-id="87409-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="87409-192">你可以使用硬件哈希仅或 OEM 名称、 序列号和模型 （在该列顺序） 或 Windows 产品 id。</span><span class="sxs-lookup"><span data-stu-id="87409-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="87409-193">你还可以使用**添加设备**旁边的链接中提供的示例.csv 文件创建设备列表。</span><span class="sxs-lookup"><span data-stu-id="87409-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="87409-194">Windows Autopilot EULA 解除的信息</span><span class="sxs-lookup"><span data-stu-id="87409-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="87409-195">重要信息</span><span class="sxs-lookup"><span data-stu-id="87409-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="87409-196">Windows Autopilot 让你可以为你的客户管理的设备上配置 Windows 的自定义的安装。</span><span class="sxs-lookup"><span data-stu-id="87409-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="87409-197">如果要执行此操作由授权客户，可以禁止显示或隐藏设置窗口，包括 EULA （最终用户许可协议） 接受屏幕时向用户正常显示的某些设置屏幕。</span><span class="sxs-lookup"><span data-stu-id="87409-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="87409-198">通过使用此函数，表明你同意禁止显示或隐藏专为用户提供通知或条款接受的术语意味着你已获取足够许可和授权从你的客户可代表隐藏条款，并且该你，任何屏幕你的客户 （组织或单个用户以这种情况可能），同意所有通知并接受所有适用于你的客户的条款。</span><span class="sxs-lookup"><span data-stu-id="87409-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="87409-199">这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。</span><span class="sxs-lookup"><span data-stu-id="87409-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="87409-200">如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。</span><span class="sxs-lookup"><span data-stu-id="87409-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>