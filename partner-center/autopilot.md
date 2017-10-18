---
title: "利用 Windows Autopilot 简化设备设置 | 合作伙伴中心"
description: "利用 Windows AutoPilot 在合作伙伴中心内添加 Windows AutoPilot 部署配置文件以简化设备设置"
author: KPacquer
keywords: "autopilot, windows autopilot, microsoft autopilot, 零接触部署, oobe, 登录屏幕"
ms.openlocfilehash: 061ee1cedbd3bc849419044bad022ccb12ef9b9f
ms.sourcegitcommit: f4b2f1a954e865e56e89d3455f48cb6e1f80ea07
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/29/2017
---
# <a name="simplify-device-setup-with-windows-autopilot"></a><span data-ttu-id="3d201-104">利用 Windows Autopilot 简化设备设置</span><span class="sxs-lookup"><span data-stu-id="3d201-104">Simplify device setup with Windows Autopilot</span></span> 

<span data-ttu-id="3d201-105">Windows Autopilot 可在首次启动时简化和保护新 Windows 10 专业版设备的设备设置，而这只需几个步骤即可实现。</span><span class="sxs-lookup"><span data-stu-id="3d201-105">Windows Autopilot streamlines and secures device setup for new Windows 10 Pro devices from first boot in only a few steps.</span></span> <span data-ttu-id="3d201-106">若要了解详细信息，请参阅 [Windows AutoPilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)。</span><span class="sxs-lookup"><span data-stu-id="3d201-106">To learn more, see [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span>

## <a name="features"></a><span data-ttu-id="3d201-107">功能</span><span class="sxs-lookup"><span data-stu-id="3d201-107">Features</span></span>

*  <span data-ttu-id="3d201-108">对设置设备的最终用户**禁用本地管理员权限**</span><span class="sxs-lookup"><span data-stu-id="3d201-108">**Disable local administrator permissions** for the end users setting up devices</span></span>
*  <span data-ttu-id="3d201-109">**显示组织的登录页面**。</span><span class="sxs-lookup"><span data-stu-id="3d201-109">**Show an organization's login page**.</span></span> <span data-ttu-id="3d201-110">组织可以预定义登录页面，以将设备添加为工作设备，并使用 Azure Active Directory 加入设备。</span><span class="sxs-lookup"><span data-stu-id="3d201-110">The organization can predefine a logon page that adds the device as a work device, and joins the device with Azure Active Directory.</span></span>
*  <span data-ttu-id="3d201-111">在 OOBE 完成后，**将设备注册到 Mobile Device Manager (MDM) 中**，例如 Microsoft Intune。</span><span class="sxs-lookup"><span data-stu-id="3d201-111">**Enroll the device into a Mobile Device Manager (MDM)**, for example: Microsoft Intune, after OOBE is complete.</span></span>
*  <span data-ttu-id="3d201-112">利用 Windows AutoPilot 部署配置文件，**简化全新安装体验 (OOBE)**，以仅使用所需的步骤和决策。</span><span class="sxs-lookup"><span data-stu-id="3d201-112">**Streamline the out-of-box experience (OOBE)** to use just the steps and decisions required, using a Windows AutoPilot Deployment profile.</span></span> 

## <a name="requirements"></a><span data-ttu-id="3d201-113">要求</span><span class="sxs-lookup"><span data-stu-id="3d201-113">Requirements</span></span>

*  <span data-ttu-id="3d201-114">设备预安装 Windows 10 专业版创意者更新（1703 或更高版本）或支持高级 PC 的 Windows 10 专业版。</span><span class="sxs-lookup"><span data-stu-id="3d201-114">Devices pre-installed with Windows 10 Pro Creators Update (version 1703 or later) or Windows 10 Pro for Advanced PCs.</span></span>
*  <span data-ttu-id="3d201-115">称为硬件哈希值（128 HWH 或 4k HWH）的设备标识符，这通常由 OEM 提供。</span><span class="sxs-lookup"><span data-stu-id="3d201-115">Device identifier known as a hardware hash (128 HWH or 4k HWH), which is typically provided by an OEM.</span></span> <span data-ttu-id="3d201-116">你将使用标识符分配合作伙伴中心内的组织配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-116">You'll use identifiers to assign organization profiles in Partner Center.</span></span> <span data-ttu-id="3d201-117">2017 年 9 月后，你将不再需要硬件哈希。</span><span class="sxs-lookup"><span data-stu-id="3d201-117">After September 2017 you will no longer need the hardware hash.</span></span> 
*  <span data-ttu-id="3d201-118">设备必须可访问 Internet。</span><span class="sxs-lookup"><span data-stu-id="3d201-118">The devices must have access to the internet.</span></span> <span data-ttu-id="3d201-119">设备如果无法连接，则显示默认的 Windows 全新安装体验 (OOBE) 屏幕。</span><span class="sxs-lookup"><span data-stu-id="3d201-119">When the device can’t connect, it shows the default Windows out-of-box experience (OOBE) screens.</span></span>
*  <span data-ttu-id="3d201-120">将设备注册到 MDM 需要 Azure Active Directory Premium。</span><span class="sxs-lookup"><span data-stu-id="3d201-120">Enrolling the device into an MDM requires Azure Active Directory Premium.</span></span>

## <a name="add-organization-login-pages-to-oobe"></a><span data-ttu-id="3d201-121">向 OOBE 中添加组织登录页面</span><span class="sxs-lookup"><span data-stu-id="3d201-121">Add organization login pages to OOBE</span></span>

<span data-ttu-id="3d201-122">若要添加特定于组织的页面，请将设备添加到贵组织的 [Azure AD 目录](https://go.microsoft.com/fwlink/?linkid=848958)，并创建登录页面。</span><span class="sxs-lookup"><span data-stu-id="3d201-122">To add organization-specific pages, add the devices into your organization’s [Azure AD directory](https://go.microsoft.com/fwlink/?linkid=848958) and create login pages.</span></span>


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="3d201-123">利用 Windows AutoPilot 部署配置文件从 OOBE 中删除 Windows 页面</span><span class="sxs-lookup"><span data-stu-id="3d201-123">Remove Windows pages from OOBE with a Windows AutoPilot deployment profile</span></span>

### <a name="examples-of-settings-in-a-windows-autopilot-deployment-profile"></a><span data-ttu-id="3d201-124">Windows AutoPilot 部署配置文件中的设置示例</span><span class="sxs-lookup"><span data-stu-id="3d201-124">Examples of settings in a Windows AutoPilot deployment profile</span></span>
*  <span data-ttu-id="3d201-125">在设置中跳过“隐私设置”</span><span class="sxs-lookup"><span data-stu-id="3d201-125">Skip Privacy Settings in setup</span></span>
*  <span data-ttu-id="3d201-126">在设置中禁用本地管理员帐户</span><span class="sxs-lookup"><span data-stu-id="3d201-126">Disable local admin account in setup</span></span>
*  <span data-ttu-id="3d201-127">在设置中自动跳过页面</span><span class="sxs-lookup"><span data-stu-id="3d201-127">Automatically skip pages in setup</span></span>
   *  <span data-ttu-id="3d201-128">为工作单位或学校自动选择设置</span><span class="sxs-lookup"><span data-stu-id="3d201-128">Automatically select setup for work or school</span></span>
   *  <span data-ttu-id="3d201-129">跳过 Cortana、OneDrive 和 OEM 注册设置页面</span><span class="sxs-lookup"><span data-stu-id="3d201-129">Skip Cortana, OneDrive, and OEM registration setup pages</span></span>

### <a name="add-devices-and-apply-a-profile"></a><span data-ttu-id="3d201-130">添加设备和应用配置文件</span><span class="sxs-lookup"><span data-stu-id="3d201-130">Add devices and apply a profile</span></span>

<span data-ttu-id="3d201-131">在合作伙伴中心内，可创建 Windows AutoPilot 部署配置文件，并将其应用于设备列表。</span><span class="sxs-lookup"><span data-stu-id="3d201-131">In Partner Center, you can create a Windows AutoPilot deployment profile and apply it to a list of the devices.</span></span>

<span data-ttu-id="3d201-132">若要配置设备，请将设备列表上传到合作伙伴中心，然后创建应用于设备的配置文件并应用它。</span><span class="sxs-lookup"><span data-stu-id="3d201-132">To configure devices, upload a list of the devices into Partner Center, create a profile that applies to the devices, and apply it.</span></span>

1.  <span data-ttu-id="3d201-133">将设备列表添加到合作伙伴中心内。</span><span class="sxs-lookup"><span data-stu-id="3d201-133">Add the list of devices into Partner Center.</span></span>

    <span data-ttu-id="3d201-134">（销售代理和管理员代理有权将设备列表添加到合作伙伴中心内。）</span><span class="sxs-lookup"><span data-stu-id="3d201-134">Sales agents and admin agents have access to add the list of devices into Partner Center.</span></span>
    
    <span data-ttu-id="3d201-135">间接经销商能够与他们的间接提供商合作添加此列表。</span><span class="sxs-lookup"><span data-stu-id="3d201-135">Indirect resellers can work with their indirect provider to add this.</span></span>

    <span data-ttu-id="3d201-136">a.</span><span class="sxs-lookup"><span data-stu-id="3d201-136">a.</span></span>  <span data-ttu-id="3d201-137">使用本主题中的 PowerShell 脚本创建 .csv 文件：[Windows AutoPilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)。</span><span class="sxs-lookup"><span data-stu-id="3d201-137">Create a .csv file using the PowerShell script from the topic: [Overview of Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).</span></span> <span data-ttu-id="3d201-138">此 .csv 文件包含设备信息，其中包括序列号、OEM 名称、型号、产品 ID 和设备标识符。</span><span class="sxs-lookup"><span data-stu-id="3d201-138">This .csv file contains device info including the serial number, OEM name, model name, product ID and device identifier.</span></span> 

    <span data-ttu-id="3d201-139">b.</span><span class="sxs-lookup"><span data-stu-id="3d201-139">b.</span></span>  <span data-ttu-id="3d201-140">在合作伙伴中心仪表板中，转到**客户** > 选择要接收设备的客户 > **设备 > 添加设备**。</span><span class="sxs-lookup"><span data-stu-id="3d201-140">From the Partner Center dashboard, go to **Customers** > select the customer that’s receiving the devices > **Devices > Add devices**.</span></span>

    <span data-ttu-id="3d201-141">c.</span><span class="sxs-lookup"><span data-stu-id="3d201-141">c.</span></span>  <span data-ttu-id="3d201-142">命名设备的批次，例如“Contoso 销售部门电脑 - 2017 年 4 月订购”。</span><span class="sxs-lookup"><span data-stu-id="3d201-142">Name the batch of devices, for example, “Contoso Sales Department PCs – April 2017 order.”</span></span> 

    <span data-ttu-id="3d201-143">d.</span><span class="sxs-lookup"><span data-stu-id="3d201-143">d.</span></span>  <span data-ttu-id="3d201-144">单击**浏览** > 选择设备信息文件 > **验证**。</span><span class="sxs-lookup"><span data-stu-id="3d201-144">Click **Browse** > select the device info file > **Validate**.</span></span>

    <span data-ttu-id="3d201-145">**注意：**如果你尝试上传 .csv 文件后收到一条错误消息，请检查该文件的格式。</span><span class="sxs-lookup"><span data-stu-id="3d201-145">**Note:** If you get an error message after trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="3d201-146">8 月之后，你可以仅使用硬件哈希，按该列顺序使用 OEM 名称、序列号和型号，或者使用 Windows 产品 ID。</span><span class="sxs-lookup"><span data-stu-id="3d201-146">After August, you can use the Hardware Hash only, or the OEM name, serial number, and model in that column order, or the Windows Product ID.</span></span> <span data-ttu-id="3d201-147">你还可以使用**添加设备**旁边的链接中提供的示例 .csv 文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-147">You can also use the sample .csv file provided from the link next to **Add devices**.</span></span>

2.  <span data-ttu-id="3d201-148">创建可应用于设备的配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-148">Create a profile that you can apply to the devices.</span></span> <span data-ttu-id="3d201-149">（只有管理员代理才有权在合作伙伴中心内创建并应用配置文件。）</span><span class="sxs-lookup"><span data-stu-id="3d201-149">(Only admin agents have access to create and apply profiles in Partner Center.)</span></span>

    <span data-ttu-id="3d201-150">a.</span><span class="sxs-lookup"><span data-stu-id="3d201-150">a.</span></span>  <span data-ttu-id="3d201-151">在**设备**中，单击**添加新的配置文件**。</span><span class="sxs-lookup"><span data-stu-id="3d201-151">From **Devices**, click **Add new profile**.</span></span>

    <span data-ttu-id="3d201-152">b.</span><span class="sxs-lookup"><span data-stu-id="3d201-152">b.</span></span>  <span data-ttu-id="3d201-153">命名配置文件，例如“Contoso 桌面配置文件 - 跳过所有 OOBE”。</span><span class="sxs-lookup"><span data-stu-id="3d201-153">Name the profile, for example, “Contoso Desktop Profile – Skip All OOBE”.</span></span>

    <span data-ttu-id="3d201-154">c.</span><span class="sxs-lookup"><span data-stu-id="3d201-154">c.</span></span>  <span data-ttu-id="3d201-155">配置 OOBE 设置。</span><span class="sxs-lookup"><span data-stu-id="3d201-155">Configure the OOBE settings.</span></span> <span data-ttu-id="3d201-156">例如，检查**在设置中跳过“快速设置”**。</span><span class="sxs-lookup"><span data-stu-id="3d201-156">For example, check **Skip Express Settings in setup**.</span></span>

    <span data-ttu-id="3d201-157">d.</span><span class="sxs-lookup"><span data-stu-id="3d201-157">d.</span></span>  <span data-ttu-id="3d201-158">单击**提交**。</span><span class="sxs-lookup"><span data-stu-id="3d201-158">Click **Submit**.</span></span>

3.  <span data-ttu-id="3d201-159">应用配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-159">Apply the profile.</span></span>

    <span data-ttu-id="3d201-160">a.</span><span class="sxs-lookup"><span data-stu-id="3d201-160">a.</span></span>  <span data-ttu-id="3d201-161">在**设备**的**分配和删除设备**窗格中，选择要配置的设备。</span><span class="sxs-lookup"><span data-stu-id="3d201-161">From **Devices**, in the **Assign and delete devices** pane, select the devices that you want to configure.</span></span> <span data-ttu-id="3d201-162">若要选择整个批次，请单击批次名称（例如“Contoso 销售部门电脑 - 2017 年 3 月订购”）旁的复选框。</span><span class="sxs-lookup"><span data-stu-id="3d201-162">To select an entire batch, click the checkbox next to the batch name (for example, “Contoso Sales Department PCs – March 2017 order”).</span></span>

    <span data-ttu-id="3d201-163">b.</span><span class="sxs-lookup"><span data-stu-id="3d201-163">b.</span></span>  <span data-ttu-id="3d201-164">单击**应用配置文件**，然后选择相关配置文件（例如“Contoso 桌面配置文件 - 跳过所有 OOBE”)。</span><span class="sxs-lookup"><span data-stu-id="3d201-164">Click **Apply profile**, and select the profile (for example, “Contoso Desktop Profile – Skip All OOBE”).</span></span> <span data-ttu-id="3d201-165">设备将在“配置文件”列中显示该配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-165">The devices will show the profile in the Profile column.</span></span>

4.  <span data-ttu-id="3d201-166">可选：通过测试查看你的配置文件是否有效。</span><span class="sxs-lookup"><span data-stu-id="3d201-166">Optional: Test to see that your profile works.</span></span>

    <span data-ttu-id="3d201-167">a.</span><span class="sxs-lookup"><span data-stu-id="3d201-167">a.</span></span>  <span data-ttu-id="3d201-168">将设备连接到网络，并将其打开。</span><span class="sxs-lookup"><span data-stu-id="3d201-168">Connect a device to the network, and turn it on.</span></span>

    <span data-ttu-id="3d201-169">b.</span><span class="sxs-lookup"><span data-stu-id="3d201-169">b.</span></span>  <span data-ttu-id="3d201-170">验证是否显示相应的 OOBE 屏幕（如果有）。</span><span class="sxs-lookup"><span data-stu-id="3d201-170">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="3d201-171">c.</span><span class="sxs-lookup"><span data-stu-id="3d201-171">c.</span></span>  <span data-ttu-id="3d201-172">若要为新用户准备设备，请完成 OOBE 体验，然后将该设备重置为其出厂默认设置。</span><span class="sxs-lookup"><span data-stu-id="3d201-172">To prepare the device for a new user, complete the OOBE experience, then reset the device to its factory default settings.</span></span>


## <a name="to-update-or-delete-a-profile"></a><span data-ttu-id="3d201-173">更新或删除配置文件</span><span class="sxs-lookup"><span data-stu-id="3d201-173">To update or delete a profile</span></span> 

<span data-ttu-id="3d201-174">将配置文件分配给设备后，可对其进行更新，即使你已将该设备提供给客户。</span><span class="sxs-lookup"><span data-stu-id="3d201-174">Once you’ve assigned a profile to a device, you can update it, even if you’ve already given the device to your customer.</span></span> <span data-ttu-id="3d201-175">当设备连接到 Internet 时，它会在 OOBE 过程中下载你的配置文件的最新版本。</span><span class="sxs-lookup"><span data-stu-id="3d201-175">When the device connects to the internet, it downloads the latest version of your profile during the OOBE process.</span></span> <span data-ttu-id="3d201-176">如果客户将其设备还原为出厂默认设置，则该设备将重新下载你的配置文件的最新更新。</span><span class="sxs-lookup"><span data-stu-id="3d201-176">If your customer restores their device to its factory default settings, the device will again download the latest updates to your profile.</span></span> 

### <a name="you-can-remove-a-profile-from-a-device"></a><span data-ttu-id="3d201-177">可从设备中删除配置文件</span><span class="sxs-lookup"><span data-stu-id="3d201-177">You can remove a profile from a device</span></span>
1. <span data-ttu-id="3d201-178">选择要从其中删除配置文件的设备（或设备的批次）。</span><span class="sxs-lookup"><span data-stu-id="3d201-178">Select the device (or batch of devices) you want to remove the profile from.</span></span> 

2. <span data-ttu-id="3d201-179">在**分配和删除设备**窗格中，选择**删除配置文件**。</span><span class="sxs-lookup"><span data-stu-id="3d201-179">In **Assign and delete devices** pane, select **Remove profile**.</span></span>

3. <span data-ttu-id="3d201-180">转到要删除的配置文件，然后将其删除。</span><span class="sxs-lookup"><span data-stu-id="3d201-180">Go to the profile you want to remove and delete it.</span></span> <span data-ttu-id="3d201-181">将从所有设备中删除该配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-181">The profile will be deleted from all devices.</span></span>

<span data-ttu-id="3d201-182">在**设备**中，选择配置文件。</span><span class="sxs-lookup"><span data-stu-id="3d201-182">From **Devices**, select the profile.</span></span> <span data-ttu-id="3d201-183">可在此处修改现有的设置。</span><span class="sxs-lookup"><span data-stu-id="3d201-183">From here, you can modify the existing settings.</span></span>

## <a name="windows-autopilot-eula-dismissal--important-information"></a><span data-ttu-id="3d201-184">Windows Autopilot EULA 解除 - 重要信息</span><span class="sxs-lookup"><span data-stu-id="3d201-184">Windows Autopilot EULA dismissal – important information</span></span>

<span data-ttu-id="3d201-185">使用此工具，你可以在为客户管理的设备上配置 Windows 的单个安装。</span><span class="sxs-lookup"><span data-stu-id="3d201-185">Using this tool allows you to configure individual installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="3d201-186">如果客户授权你进行此操作，你可以选择不显示或隐藏在设置 Windows 时向用户正常显示的某些设置屏幕，包括 EULA 接受屏幕。</span><span class="sxs-lookup"><span data-stu-id="3d201-186">If authorized to do so by the customer, you may choose to suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA acceptance screen.</span></span> 

<span data-ttu-id="3d201-187">使用此功能，即表明你同意不显示或隐藏专为用户提供通知或条款接受的任何屏幕，意味着你已从客户方获得隐藏条款的充分许可和授权，并且你已代表你的客户（组织或单个用户，根据具体情况而定）同意所有通知并接受所有对该客户适用的条款。</span><span class="sxs-lookup"><span data-stu-id="3d201-187">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="3d201-188">这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。</span><span class="sxs-lookup"><span data-stu-id="3d201-188">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="3d201-189">如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。</span><span class="sxs-lookup"><span data-stu-id="3d201-189">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>


