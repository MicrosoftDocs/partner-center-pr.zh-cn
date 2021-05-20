---
title: 自定义设备的开箱使用体验
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 在交付客户的新设备之前，可以使用 Windows Autopilot 配置文件在 OOBE 设备上自定义或预配置设备的 (体验) 。
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149819"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="ed229-103">在新设备上使用 Windows Autopilot 配置文件自定义客户的全新安装体验</span><span class="sxs-lookup"><span data-stu-id="ed229-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="ed229-104">**适当的角色**：管理员代理|全局管理员|销售代理|用户管理管理员</span><span class="sxs-lookup"><span data-stu-id="ed229-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="ed229-105">如果管理客户设备，可能需要为客户的用户自定义 (OOBE) 的开箱即用体验。</span><span class="sxs-lookup"><span data-stu-id="ed229-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="ed229-106">在将设备交付到客户之前，可以使用Windows Autopilot配置文件预配置新设备，并为客户已购买的设备应用新配置文件。</span><span class="sxs-lookup"><span data-stu-id="ed229-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="ed229-107">请注意，OEM 已开始在 Autopilot 设备框外部添加发货标签，该标签显示设备的产品密钥 ID (**PKID) 。**</span><span class="sxs-lookup"><span data-stu-id="ed229-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="ed229-108">此一维可读条形码为下游合作伙伴提供了一种为 Autopilot 注册设备的方法，而无需将设备拆箱 () 并按替代方法获取设备 ID。</span><span class="sxs-lookup"><span data-stu-id="ed229-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="ed229-109">本文介绍如何创建 Autopilot 配置文件，以及如何将 Autopilot 配置文件应用到 合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ed229-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="ed229-110">如果不熟悉 Autopilot，请查看以下文章中的信息：</span><span class="sxs-lookup"><span data-stu-id="ed229-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="ed229-111">Windows Autopilot 概述</span><span class="sxs-lookup"><span data-stu-id="ed229-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="ed229-112">Autopilot 部署参考指南</span><span class="sxs-lookup"><span data-stu-id="ed229-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="ed229-113">概述</span><span class="sxs-lookup"><span data-stu-id="ed229-113">Overview</span></span>

<span data-ttu-id="ed229-114">使用 Windows Autopilot 中的 合作伙伴中心 功能，可以创建要应用于客户设备的自定义配置文件。</span><span class="sxs-lookup"><span data-stu-id="ed229-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="ed229-115">本文发布时提供了以下配置文件设置：</span><span class="sxs-lookup"><span data-stu-id="ed229-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="ed229-116">跳过隐私设置。</span><span class="sxs-lookup"><span data-stu-id="ed229-116">Skip privacy settings.</span></span> <span data-ttu-id="ed229-117">此可选的 Autopilot 配置文件设置使组织能够在 OOBE 过程中不询问隐私设置。</span><span class="sxs-lookup"><span data-stu-id="ed229-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="ed229-118">禁用在设备上创建本地管理员帐户。</span><span class="sxs-lookup"><span data-stu-id="ed229-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="ed229-119">完成该过程后，组织可以决定设置设备的用户是否应该具有管理员访问权限。</span><span class="sxs-lookup"><span data-stu-id="ed229-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="ed229-120">自动为工作或学校设置设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="ed229-121">向 Autopilot 注册的所有设备都将自动视为工作或学校设备，因此在 OOBE 过程中不会询问此问题。</span><span class="sxs-lookup"><span data-stu-id="ed229-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="ed229-122">跳过 Cortana、OneDrive 和 OEM 注册设置页。</span><span class="sxs-lookup"><span data-stu-id="ed229-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="ed229-123">注册到 Autopilot 的所有设备都会在 (OOBE) 进程的全新体验期间自动跳过这些页面。</span><span class="sxs-lookup"><span data-stu-id="ed229-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="ed229-124"> (EULA) ，跳过最终用户许可协议。</span><span class="sxs-lookup"><span data-stu-id="ed229-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="ed229-125">从 Windows 10 版本1709开始，组织可以决定跳过 OOBE 过程中显示的 EULA 页面。</span><span class="sxs-lookup"><span data-stu-id="ed229-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="ed229-126">请参阅下面的 [Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal) ，以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。</span><span class="sxs-lookup"><span data-stu-id="ed229-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="ed229-127">以下配置文件和设备管理权限和限制适用：</span><span class="sxs-lookup"><span data-stu-id="ed229-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="ed229-128">即使客户已删除合作伙伴的委派管理权限，CSP 合作伙伴也可以继续管理与其有经销商关系的现有客户的 Autopilot 配置文件。</span><span class="sxs-lookup"><span data-stu-id="ed229-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="ed229-129">你可以管理已添加的客户的现有设备，</span><span class="sxs-lookup"><span data-stu-id="ed229-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="ed229-130">但无法管理客户已上传到适用于企业的 Microsoft Store 或 Microsoft Intune 门户的设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="ed229-131">在合作伙伴中心创建和管理 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="ed229-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="ed229-132">在合作伙伴中心，你可以创建 Windows Autopilot 部署配置文件并将它们应用到设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="ed229-133">只有管理代理可以创建和应用配置文件。</span><span class="sxs-lookup"><span data-stu-id="ed229-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="ed229-134">创建新的 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="ed229-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="ed229-135">从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要为其创建 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="ed229-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="ed229-136">在客户的详细信息页上，选择 " **设备**"。</span><span class="sxs-lookup"><span data-stu-id="ed229-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ed229-137">在 " **Windows Autopilot 配置文件** " 下，选择 " **添加新配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="ed229-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="ed229-138">输入配置文件的 "名称" 和 "说明"，然后配置 "OOBE" 设置。</span><span class="sxs-lookup"><span data-stu-id="ed229-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="ed229-139">选择：</span><span class="sxs-lookup"><span data-stu-id="ed229-139">Choose from:</span></span>  

   - <span data-ttu-id="ed229-140">在安装程序中跳过隐私设置</span><span class="sxs-lookup"><span data-stu-id="ed229-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="ed229-141">在设置中禁用本地管理员帐户</span><span class="sxs-lookup"><span data-stu-id="ed229-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="ed229-142">在设置中自动跳过页面</span><span class="sxs-lookup"><span data-stu-id="ed229-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="ed229-143"> (包括 *自动选择适用于工作或学校的设置* ，并 *跳过 Cortana、OneDrive 和 OEM 注册设置页*) </span><span class="sxs-lookup"><span data-stu-id="ed229-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="ed229-144">跳过最终用户许可协议 (EULA) </span><span class="sxs-lookup"><span data-stu-id="ed229-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="ed229-145">请参阅下面的 [Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal) ，以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。</span><span class="sxs-lookup"><span data-stu-id="ed229-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="ed229-146">完成后选择 **提交**。</span><span class="sxs-lookup"><span data-stu-id="ed229-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="ed229-147">将 Autopilot 配置文件应用到客户设备</span><span class="sxs-lookup"><span data-stu-id="ed229-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="ed229-148">以下说明假定您已将客户的设备添加到合作伙伴中心，并且您可以访问其设备列表。</span><span class="sxs-lookup"><span data-stu-id="ed229-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="ed229-149">如果尚未添加客户的设备，请按照 [将设备添加到客户帐户](#add-devices-to-a-customers-account) 中的说明操作，然后执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="ed229-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="ed229-150">为客户创建 Autopilot 配置文件后，可将其应用到客户的设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="ed229-151">从 **"** 客户"菜单中合作伙伴中心"客户"，然后选择创建 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="ed229-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="ed229-152">在客户的详细信息页上，选择"**设备"。**</span><span class="sxs-lookup"><span data-stu-id="ed229-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ed229-153">在 **"将配置文件应用于设备**"下，选择要将配置文件添加到的设备或设备组，然后选择"应用 **配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="ed229-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="ed229-154">刚刚应用的配置文件将显示在"配置文件 **"** 列中。</span><span class="sxs-lookup"><span data-stu-id="ed229-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="ed229-155">按照以下步骤验证配置文件是否成功应用于设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="ed229-156">a.</span><span class="sxs-lookup"><span data-stu-id="ed229-156">a.</span></span>  <span data-ttu-id="ed229-157">将设备连接到网络并打开它。</span><span class="sxs-lookup"><span data-stu-id="ed229-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="ed229-158">b.</span><span class="sxs-lookup"><span data-stu-id="ed229-158">b.</span></span>  <span data-ttu-id="ed229-159">验证是否显示相应的 OOBE 屏幕（如果有）。</span><span class="sxs-lookup"><span data-stu-id="ed229-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="ed229-160">c.</span><span class="sxs-lookup"><span data-stu-id="ed229-160">c.</span></span>  <span data-ttu-id="ed229-161">当 OOBE 进程停止时，将设备重置为出厂默认设置，为新用户做好准备。</span><span class="sxs-lookup"><span data-stu-id="ed229-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="ed229-162">从客户的设备中删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="ed229-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="ed229-163">从 **"** 客户"菜单中合作伙伴中心"客户"，然后选择创建 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="ed229-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="ed229-164">在客户的详细信息页上，选择"**设备"。**</span><span class="sxs-lookup"><span data-stu-id="ed229-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ed229-165">在 **"将配置文件应用到设备**"下，选择要从中删除配置文件的设备，然后选择"**删除配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="ed229-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="ed229-166">从设备中删除配置文件不会从列表中删除该配置文件。</span><span class="sxs-lookup"><span data-stu-id="ed229-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="ed229-167">如果要删除配置文件，请按照更新或删除 [Autopilot 配置文件 中的说明操作](#update-or-delete-an-autopilot-profile)。</span><span class="sxs-lookup"><span data-stu-id="ed229-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="ed229-168">更新或删除 Autopilot 配置文件</span><span class="sxs-lookup"><span data-stu-id="ed229-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="ed229-169">如果客户想要在将设备交付到客户后更改开箱即用体验，可以在 合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="ed229-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="ed229-170">当客户的设备连接到 Internet 时，它将在 OOBE 过程中下载最新的配置文件版本。</span><span class="sxs-lookup"><span data-stu-id="ed229-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="ed229-171">此外，客户每次将设备还原到出厂默认设置时，设备都会在 OOBE 过程中再次下载最新的配置文件版本。</span><span class="sxs-lookup"><span data-stu-id="ed229-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="ed229-172">从 **"** 客户合作伙伴中心选择"客户"，然后选择想要更改 Autopilot 配置文件的客户。</span><span class="sxs-lookup"><span data-stu-id="ed229-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="ed229-173">在客户的详细信息页上，选择"**设备"。**</span><span class="sxs-lookup"><span data-stu-id="ed229-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ed229-174">在 **Windows Autopilot配置文件** "下，选择需要更新的配置文件。</span><span class="sxs-lookup"><span data-stu-id="ed229-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="ed229-175">进行所需的更改，然后选择 " **提交**"。</span><span class="sxs-lookup"><span data-stu-id="ed229-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="ed229-176">若要删除此配置文件，请选择页面右上角的 " **删除配置文件** "。</span><span class="sxs-lookup"><span data-stu-id="ed229-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="ed229-177">向客户帐户添加设备</span><span class="sxs-lookup"><span data-stu-id="ed229-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="ed229-178">销售代理和管理代理可以将设备添加到客户的帐户。</span><span class="sxs-lookup"><span data-stu-id="ed229-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="ed229-179">你必须能够访问客户的设备列表，然后才能将自定义 Autopilot 配置文件应用到客户设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="ed229-180">如果计划使用 OEM 名称、序列号和型号组合，请注意以下限制：</span><span class="sxs-lookup"><span data-stu-id="ed229-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="ed229-181">此元组仅适用于 (4k 哈希的较新设备，例如) ，不支持 (RS2 和之前的设备) 的128b 哈希。</span><span class="sxs-lookup"><span data-stu-id="ed229-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="ed229-182">元组注册区分大小写，因此文件中的数据必须与 OEM 提供商)  (硬件提供程序提供的名称 ***完全*** 匹配。</span><span class="sxs-lookup"><span data-stu-id="ed229-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="ed229-183">按照以下说明将设备添加到合作伙伴中心的客户帐户。</span><span class="sxs-lookup"><span data-stu-id="ed229-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="ed229-184">从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要管理其设备的客户。</span><span class="sxs-lookup"><span data-stu-id="ed229-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="ed229-185">在客户的详细信息页上，选择 " **设备**"。</span><span class="sxs-lookup"><span data-stu-id="ed229-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="ed229-186">在 " **将配置文件应用到设备** " 下选择 " **添加设备**"。</span><span class="sxs-lookup"><span data-stu-id="ed229-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="ed229-187">输入设备列表的名称，然后选择 " **浏览** "，将客户列表 (以 .csv 文件格式) 到 "合作伙伴中心" 上传。</span><span class="sxs-lookup"><span data-stu-id="ed229-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ed229-188">你应收到此 .csv 文件，并购买你的设备。</span><span class="sxs-lookup"><span data-stu-id="ed229-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="ed229-189">如果未收到 .csv 文件，则可以按照 [向 Windows Autopilot 中添加设备](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步骤自行创建。</span><span class="sxs-lookup"><span data-stu-id="ed229-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="ed229-190">上传 .csv 文件，然后选择 " **保存**"。</span><span class="sxs-lookup"><span data-stu-id="ed229-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="ed229-191">如果在尝试上传 .csv 文件时收到错误消息，请检查该文件的格式。</span><span class="sxs-lookup"><span data-stu-id="ed229-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="ed229-192">可以仅使用硬件哈希，也可使用 OEM 名称、序列号和型号（按列顺序），还可使用 Windows 产品 ID。</span><span class="sxs-lookup"><span data-stu-id="ed229-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="ed229-193">你还可以使用 " **添加设备** " 下的链接中提供的示例 .csv 文件来创建设备列表。</span><span class="sxs-lookup"><span data-stu-id="ed229-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="ed229-194">.Csv 文件应如下所示：</span><span class="sxs-lookup"><span data-stu-id="ed229-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="ed229-195">**设备序列号、Windows 产品 ID、硬件哈希、制造商名称、设备型号**</span><span class="sxs-lookup"><span data-stu-id="ed229-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="ed229-196">**{serialNumber},,, Microsoft Corporation，Surface 便携机**</span><span class="sxs-lookup"><span data-stu-id="ed229-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="ed229-197">"制造商名称" 和 "设备型号" 区分大小写。</span><span class="sxs-lookup"><span data-stu-id="ed229-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="ed229-198">如果不知道为"制造商名称"和"设备型号"设置什么值，可以在设备上运行此代码以收集正确的值：</span><span class="sxs-lookup"><span data-stu-id="ed229-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="ed229-199">Windows Autopilot EULA 解除</span><span class="sxs-lookup"><span data-stu-id="ed229-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="ed229-200">重要信息</span><span class="sxs-lookup"><span data-stu-id="ed229-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="ed229-201">Windows Autopilot允许你在为客户管理的设备上配置 Windows 的自定义安装。</span><span class="sxs-lookup"><span data-stu-id="ed229-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="ed229-202">如果客户授权这样做，可以取消或隐藏在设置 Windows 时通常呈现给用户的某些设置屏幕，包括"EULA (最终用户许可协议") 接受屏幕。</span><span class="sxs-lookup"><span data-stu-id="ed229-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="ed229-203">使用此函数即表示你同意禁止或隐藏旨在为用户提供通知或接受条款的任何屏幕意味着你已获得客户的足够许可和授权来隐藏条款，并且你代表你的客户 (无论组织还是个人用户（在这种情况下) 都同意任何通知并接受适用于你的客户的任何条款。</span><span class="sxs-lookup"><span data-stu-id="ed229-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="ed229-204">这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。</span><span class="sxs-lookup"><span data-stu-id="ed229-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="ed229-205">如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。</span><span class="sxs-lookup"><span data-stu-id="ed229-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>