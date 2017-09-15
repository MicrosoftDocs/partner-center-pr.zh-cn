---
title: Simplify device setup with Windows Autopilot | Partner Center
description: Add a Windows AutoPilot deployment profile in Partner Center to simplify device setup with Windows Autopilot
author: KPacquer
keywords: autopilot, windows autopilot, microsoft autopilot, zero-touch deployment, oobe, login screens
ms.openlocfilehash: a307a1e8f46137ba0f796b2ad2fb059c1d602eac
ms.sourcegitcommit: 493122887ab9a5524590be12f5e1fedf4a004682
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/28/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a><span data-ttu-id="03768-104">Simplify device setup with Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="03768-104">Simplify device setup with Windows Autopilot</span></span> 

<span data-ttu-id="03768-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span><span class="sxs-lookup"><span data-stu-id="03768-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span></span> <span data-ttu-id="03768-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span><span class="sxs-lookup"><span data-stu-id="03768-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span>

## <a name="features"></a><span data-ttu-id="03768-107">Features</span><span class="sxs-lookup"><span data-stu-id="03768-107">Features</span></span>

*  <span data-ttu-id="03768-108">**Disable local administrator permissions** for the end users setting up devices</span><span class="sxs-lookup"><span data-stu-id="03768-108">**Disable local administrator permissions** for the end users setting up devices</span></span>
*  <span data-ttu-id="03768-109">**Show an organization's login page**.</span><span class="sxs-lookup"><span data-stu-id="03768-109">**Show an organization's login page**.</span></span> <span data-ttu-id="03768-110">The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="03768-110">The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span></span>
*  <span data-ttu-id="03768-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span><span class="sxs-lookup"><span data-stu-id="03768-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span></span>
*  <span data-ttu-id="03768-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span><span class="sxs-lookup"><span data-stu-id="03768-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span></span> 

## <a name="requirements"></a><span data-ttu-id="03768-113">Requirements</span><span class="sxs-lookup"><span data-stu-id="03768-113">Requirements</span></span>

*  <span data-ttu-id="03768-114">设备预安装 Windows 10 专业版创意者更新（1703 或更高版本）或支持高级 PC 的 Windows 10 专业版。</span><span class="sxs-lookup"><span data-stu-id="03768-114">Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later) or Windows 10 Pro for Advanced PCs.</span></span>
*  <span data-ttu-id="03768-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span><span class="sxs-lookup"><span data-stu-id="03768-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span></span> <span data-ttu-id="03768-116">You'll use identifiers to assign organization profiles in Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03768-116">You'll use identifiers to assign organization profiles in Partner Center.</span></span> <span data-ttu-id="03768-117">2017 年 9 月后，你将不再需要硬件哈希。</span><span class="sxs-lookup"><span data-stu-id="03768-117">After September 2017 you will no longer need the hardware hash.</span></span> 
*  <span data-ttu-id="03768-118">The devices must have access to the internet.</span><span class="sxs-lookup"><span data-stu-id="03768-118">The devices must have access to the internet.</span></span> <span data-ttu-id="03768-119">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span><span class="sxs-lookup"><span data-stu-id="03768-119">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span></span>
*  <span data-ttu-id="03768-120">Enrolling the device into an MDM requires Azure Active Directory Premium.</span><span class="sxs-lookup"><span data-stu-id="03768-120">Enrolling the device into an MDM requires Azure Active Directory Premium.</span></span>

## <a name="add-organization-login-pages-to-oobe"></a><span data-ttu-id="03768-121">Add organization login pages to OOBE</span><span class="sxs-lookup"><span data-stu-id="03768-121">Add organization login pages to OOBE</span></span>

<span data-ttu-id="03768-122">To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span><span class="sxs-lookup"><span data-stu-id="03768-122">To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span></span>


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="03768-123">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span><span class="sxs-lookup"><span data-stu-id="03768-123">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span></span>

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="03768-124">Examples of settings in a Windows AutoPilot deployment profile</span><span class="sxs-lookup"><span data-stu-id="03768-124">Examples of settings in a Windows AutoPilot deployment profile</span></span>
*  <span data-ttu-id="03768-125">Skip Privacy Settings in setup</span><span class="sxs-lookup"><span data-stu-id="03768-125">Skip Privacy Settings in setup</span></span>
*  <span data-ttu-id="03768-126">Disable local admin account in setup</span><span class="sxs-lookup"><span data-stu-id="03768-126">Disable local admin account in setup</span></span>
*  <span data-ttu-id="03768-127">Automatically skip pages in setup</span><span class="sxs-lookup"><span data-stu-id="03768-127">Automatically skip pages in setup</span></span>
   *  <span data-ttu-id="03768-128">Automatically select setup for work or school</span><span class="sxs-lookup"><span data-stu-id="03768-128">Automatically select setup for work or school</span></span>
   *  <span data-ttu-id="03768-129">Skip Cortana, OneDrive, and OEM registration setup pages</span><span class="sxs-lookup"><span data-stu-id="03768-129">Skip Cortana, OneDrive, and OEM registration setup pages</span></span>

### <a name="add-devices-and-apply-a-profile"></a><span data-ttu-id="03768-130">Add devices and apply a profile</span><span class="sxs-lookup"><span data-stu-id="03768-130">Add devices and apply a profile</span></span>

<span data-ttu-id="03768-131">In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span><span class="sxs-lookup"><span data-stu-id="03768-131">In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span></span>

<span data-ttu-id="03768-132">To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.</span><span class="sxs-lookup"><span data-stu-id="03768-132">To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.</span></span>

1.  <span data-ttu-id="03768-133">Add the list of devices into Partner Center.</span><span class="sxs-lookup"><span data-stu-id="03768-133">Add the list of devices into Partner Center.</span></span>

    <span data-ttu-id="03768-134">（销售代理和管理员代理有权将设备列表添加到合作伙伴中心内。）</span><span class="sxs-lookup"><span data-stu-id="03768-134">Sales agents and admin agents have access to add the list of devices into Partner Center.</span></span>
    
    <span data-ttu-id="03768-135">间接经销商能够与他们的间接提供商合作添加此列表。</span><span class="sxs-lookup"><span data-stu-id="03768-135">Indirect resellers can work with their indirect provider to add this.</span></span>

    <span data-ttu-id="03768-136">a.</span><span class="sxs-lookup"><span data-stu-id="03768-136">a.</span></span>  <span data-ttu-id="03768-137">Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span><span class="sxs-lookup"><span data-stu-id="03768-137">Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span> <span data-ttu-id="03768-138">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span><span class="sxs-lookup"><span data-stu-id="03768-138">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span></span> 

    <span data-ttu-id="03768-139">b.</span><span class="sxs-lookup"><span data-stu-id="03768-139">b.</span></span>  <span data-ttu-id="03768-140">From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span><span class="sxs-lookup"><span data-stu-id="03768-140">From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span></span>

    <span data-ttu-id="03768-141">c.</span><span class="sxs-lookup"><span data-stu-id="03768-141">c.</span></span>  <span data-ttu-id="03768-142">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span><span class="sxs-lookup"><span data-stu-id="03768-142">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span></span> 

    <span data-ttu-id="03768-143">d.</span><span class="sxs-lookup"><span data-stu-id="03768-143">d.</span></span>  <span data-ttu-id="03768-144">Click **Browse** > select the device info file > **Validate**.</span><span class="sxs-lookup"><span data-stu-id="03768-144">Click **Browse** > select the device info file > **Validate**.</span></span>

    <span data-ttu-id="03768-145">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span><span class="sxs-lookup"><span data-stu-id="03768-145">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="03768-146">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span><span class="sxs-lookup"><span data-stu-id="03768-146">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span></span> <span data-ttu-id="03768-147">You can also use the sample .csv file provided from the link next to **Add devices**.</span><span class="sxs-lookup"><span data-stu-id="03768-147">You can also use the sample .csv file provided from the link next to **Add devices**.</span></span>

2.  <span data-ttu-id="03768-148">Create a profile that you can apply to the devices.</span><span class="sxs-lookup"><span data-stu-id="03768-148">Create a profile that you can apply to the devices.</span></span> <span data-ttu-id="03768-149">(Only admin agents have access to create and apply profiles in Partner Center.)</span><span class="sxs-lookup"><span data-stu-id="03768-149">(Only admin agents have access to create and apply profiles in Partner Center.)</span></span>

    <span data-ttu-id="03768-150">a.</span><span class="sxs-lookup"><span data-stu-id="03768-150">a.</span></span>  <span data-ttu-id="03768-151">From **Devices**, click **Add new profile**.</span><span class="sxs-lookup"><span data-stu-id="03768-151">From **Devices**, click **Add new profile**.</span></span>

    <span data-ttu-id="03768-152">b.</span><span class="sxs-lookup"><span data-stu-id="03768-152">b.</span></span>  <span data-ttu-id="03768-153">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span><span class="sxs-lookup"><span data-stu-id="03768-153">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span></span>

    <span data-ttu-id="03768-154">c.</span><span class="sxs-lookup"><span data-stu-id="03768-154">c.</span></span>  <span data-ttu-id="03768-155">Configure the OOBE settings.</span><span class="sxs-lookup"><span data-stu-id="03768-155">Configure the OOBE settings.</span></span> <span data-ttu-id="03768-156">For example, check **Skip Express Settings in setup**.</span><span class="sxs-lookup"><span data-stu-id="03768-156">For example, check **Skip Express Settings in setup**.</span></span>

    <span data-ttu-id="03768-157">d.</span><span class="sxs-lookup"><span data-stu-id="03768-157">d.</span></span>  <span data-ttu-id="03768-158">Click **Submit**.</span><span class="sxs-lookup"><span data-stu-id="03768-158">Click **Submit**.</span></span>

3.  <span data-ttu-id="03768-159">Apply the profile.</span><span class="sxs-lookup"><span data-stu-id="03768-159">Apply the profile.</span></span>

    <span data-ttu-id="03768-160">a.</span><span class="sxs-lookup"><span data-stu-id="03768-160">a.</span></span>  <span data-ttu-id="03768-161">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span><span class="sxs-lookup"><span data-stu-id="03768-161">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span></span> <span data-ttu-id="03768-162">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span><span class="sxs-lookup"><span data-stu-id="03768-162">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span></span>

    <span data-ttu-id="03768-163">b.</span><span class="sxs-lookup"><span data-stu-id="03768-163">b.</span></span>  <span data-ttu-id="03768-164">Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span><span class="sxs-lookup"><span data-stu-id="03768-164">Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span></span> <span data-ttu-id="03768-165">The devices will show the profile in the Profile column.</span><span class="sxs-lookup"><span data-stu-id="03768-165">The devices will show the profile in the Profile column.</span></span>

4.  <span data-ttu-id="03768-166">Optional: Test to see that your profile works.</span><span class="sxs-lookup"><span data-stu-id="03768-166">Optional: Test to see that your profile works.</span></span>

    <span data-ttu-id="03768-167">a.</span><span class="sxs-lookup"><span data-stu-id="03768-167">a.</span></span>  <span data-ttu-id="03768-168">Connect a device to the network, and turn it on.</span><span class="sxs-lookup"><span data-stu-id="03768-168">Connect a device to the network, and turn it on.</span></span>

    <span data-ttu-id="03768-169">b.</span><span class="sxs-lookup"><span data-stu-id="03768-169">b.</span></span>  <span data-ttu-id="03768-170">Verify that the appropriate OOBE screens (if any) appear.</span><span class="sxs-lookup"><span data-stu-id="03768-170">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="03768-171">c.</span><span class="sxs-lookup"><span data-stu-id="03768-171">c.</span></span>  <span data-ttu-id="03768-172">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span><span class="sxs-lookup"><span data-stu-id="03768-172">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span></span>


## <a name="to-update-or-delete-a-profile"></a><span data-ttu-id="03768-173">To update or delete a profile</span><span class="sxs-lookup"><span data-stu-id="03768-173">To update or delete a profile</span></span> 

<span data-ttu-id="03768-174">Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span><span class="sxs-lookup"><span data-stu-id="03768-174">Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span></span> <span data-ttu-id="03768-175">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span><span class="sxs-lookup"><span data-stu-id="03768-175">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span></span> <span data-ttu-id="03768-176">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span><span class="sxs-lookup"><span data-stu-id="03768-176">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 

### <a name="you-can-remove-a-profile-from-a-device"></a><span data-ttu-id="03768-177">You can remove a profile from a device</span><span class="sxs-lookup"><span data-stu-id="03768-177">You can remove a profile from a device</span></span>
1. <span data-ttu-id="03768-178">Select the device (or batch of devices) you want to remove the profile from.</span><span class="sxs-lookup"><span data-stu-id="03768-178">Select the device (or batch of devices) you want to remove the profile from.</span></span> 

2. <span data-ttu-id="03768-179">In **Assign and delete devices** pane, select **Remove profile**.</span><span class="sxs-lookup"><span data-stu-id="03768-179">In **Assign and delete devices** pane, select **Remove profile**.</span></span>

3. <span data-ttu-id="03768-180">Go to the profile you want to remove and delete it.</span><span class="sxs-lookup"><span data-stu-id="03768-180">Go to the profile you want to remove and delete it.</span></span> <span data-ttu-id="03768-181">The profile will be deleted from all devices.</span><span class="sxs-lookup"><span data-stu-id="03768-181">The profile will be deleted from all devices.</span></span>

<span data-ttu-id="03768-182">From **Devices**, select the profile.</span><span class="sxs-lookup"><span data-stu-id="03768-182">From **Devices**, select the profile.</span></span> <span data-ttu-id="03768-183">From here, you can modify the existing settings.</span><span class="sxs-lookup"><span data-stu-id="03768-183">From here, you can modify the existing settings.</span></span>

