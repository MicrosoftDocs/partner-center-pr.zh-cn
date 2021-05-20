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
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>在新设备上使用 Windows Autopilot 配置文件自定义客户的全新安装体验

**适当的角色**：管理员代理|全局管理员|销售代理|用户管理管理员

如果管理客户设备，可能需要为客户的用户自定义 (OOBE) 的开箱即用体验。 在将设备交付到客户之前，可以使用Windows Autopilot配置文件预配置新设备，并为客户已购买的设备应用新配置文件。 

请注意，OEM 已开始在 Autopilot 设备框外部添加发货标签，该标签显示设备的产品密钥 ID (**PKID) 。**  此一维可读条形码为下游合作伙伴提供了一种为 Autopilot 注册设备的方法，而无需将设备拆箱 () 并按替代方法获取设备 ID。

本文介绍如何创建 Autopilot 配置文件，以及如何将 Autopilot 配置文件应用到 合作伙伴中心。

如果不熟悉 Autopilot，请查看以下文章中的信息：

- [Windows Autopilot 概述](/windows/deployment/windows-10-auto-pilot)
- [Autopilot 部署参考指南](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概述

使用 Windows Autopilot 中的 合作伙伴中心 功能，可以创建要应用于客户设备的自定义配置文件。 本文发布时提供了以下配置文件设置：

- 跳过隐私设置。 此可选的 Autopilot 配置文件设置使组织能够在 OOBE 过程中不询问隐私设置。

- 禁用在设备上创建本地管理员帐户。 完成该过程后，组织可以决定设置设备的用户是否应该具有管理员访问权限。

- 自动为工作或学校设置设备。 向 Autopilot 注册的所有设备都将自动视为工作或学校设备，因此在 OOBE 过程中不会询问此问题。

- 跳过 Cortana、OneDrive 和 OEM 注册设置页。 注册到 Autopilot 的所有设备都会在 (OOBE) 进程的全新体验期间自动跳过这些页面。

-  (EULA) ，跳过最终用户许可协议。 从 Windows 10 版本1709开始，组织可以决定跳过 OOBE 过程中显示的 EULA 页面。 请参阅下面的 [Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal) ，以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。

以下配置文件和设备管理权限和限制适用：

- 即使客户已删除合作伙伴的委派管理权限，CSP 合作伙伴也可以继续管理与其有经销商关系的现有客户的 Autopilot 配置文件。

- 你可以管理已添加的客户的现有设备，

- 但无法管理客户已上传到适用于企业的 Microsoft Store 或 Microsoft Intune 门户的设备。

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>在合作伙伴中心创建和管理 Autopilot 配置文件

在合作伙伴中心，你可以创建 Windows Autopilot 部署配置文件并将它们应用到设备。

>[!NOTE]
>只有管理代理可以创建和应用配置文件。

### <a name="create-a-new-autopilot-profile"></a>创建新的 Autopilot 配置文件

1. 从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要为其创建 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择 " **设备**"。

3. 在 " **Windows Autopilot 配置文件** " 下，选择 " **添加新配置文件**"。

4. 输入配置文件的 "名称" 和 "说明"，然后配置 "OOBE" 设置。 选择：  

   - 在安装程序中跳过隐私设置

   - 在设置中禁用本地管理员帐户
  
   - 在设置中自动跳过页面<br>
         (包括 *自动选择适用于工作或学校的设置* ，并 *跳过 Cortana、OneDrive 和 OEM 注册设置页*) 
  
   - 跳过最终用户许可协议 (EULA) <br> 
       >[!IMPORTANT] 
       >请参阅下面的 [Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal) ，以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。

5. 完成后选择 **提交**。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>将 Autopilot 配置文件应用到客户设备

>[!NOTE]
>以下说明假定您已将客户的设备添加到合作伙伴中心，并且您可以访问其设备列表。 如果尚未添加客户的设备，请按照 [将设备添加到客户帐户](#add-devices-to-a-customers-account) 中的说明操作，然后执行以下步骤。

为客户创建 Autopilot 配置文件后，可将其应用到客户的设备。

1. 从 **"** 客户"菜单中合作伙伴中心"客户"，然后选择创建 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择"**设备"。**

3. 在 **"将配置文件应用于设备**"下，选择要将配置文件添加到的设备或设备组，然后选择"应用 **配置文件"。** 刚刚应用的配置文件将显示在"配置文件 **"** 列中。

4. 按照以下步骤验证配置文件是否成功应用于设备。

    a.  将设备连接到网络并打开它。

    b.  验证是否显示相应的 OOBE 屏幕（如果有）。

    c.  当 OOBE 进程停止时，将设备重置为出厂默认设置，为新用户做好准备。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>从客户的设备中删除 Autopilot 配置文件

1. 从 **"** 客户"菜单中合作伙伴中心"客户"，然后选择创建 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择"**设备"。**

3. 在 **"将配置文件应用到设备**"下，选择要从中删除配置文件的设备，然后选择"**删除配置文件"。**

   >[!NOTE]
   >从设备中删除配置文件不会从列表中删除该配置文件。 如果要删除配置文件，请按照更新或删除 [Autopilot 配置文件 中的说明操作](#update-or-delete-an-autopilot-profile)。

### <a name="update-or-delete-an-autopilot-profile"></a>更新或删除 Autopilot 配置文件

如果客户想要在将设备交付到客户后更改开箱即用体验，可以在 合作伙伴中心。

当客户的设备连接到 Internet 时，它将在 OOBE 过程中下载最新的配置文件版本。 此外，客户每次将设备还原到出厂默认设置时，设备都会在 OOBE 过程中再次下载最新的配置文件版本。

1. 从 **"** 客户合作伙伴中心选择"客户"，然后选择想要更改 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择"**设备"。**

3. 在 **Windows Autopilot配置文件** "下，选择需要更新的配置文件。 进行所需的更改，然后选择 " **提交**"。

若要删除此配置文件，请选择页面右上角的 " **删除配置文件** "。

### <a name="add-devices-to-a-customers-account"></a>向客户帐户添加设备

>[!NOTE]
>销售代理和管理代理可以将设备添加到客户的帐户。

你必须能够访问客户的设备列表，然后才能将自定义 Autopilot 配置文件应用到客户设备。

如果计划使用 OEM 名称、序列号和型号组合，请注意以下限制：

- 此元组仅适用于 (4k 哈希的较新设备，例如) ，不支持 (RS2 和之前的设备) 的128b 哈希。

- 元组注册区分大小写，因此文件中的数据必须与 OEM 提供商)  (硬件提供程序提供的名称 ***完全*** 匹配。

按照以下说明将设备添加到合作伙伴中心的客户帐户。

1. 从 "合作伙伴中心" 菜单中选择 " **客户** "，然后选择要管理其设备的客户。

2. 在客户的详细信息页上，选择 " **设备**"。

3. 在 " **将配置文件应用到设备** " 下选择 " **添加设备**"。

4. 输入设备列表的名称，然后选择 " **浏览** "，将客户列表 (以 .csv 文件格式) 到 "合作伙伴中心" 上传。

    >[!NOTE]
    >你应收到此 .csv 文件，并购买你的设备。 如果未收到 .csv 文件，则可以按照 [向 Windows Autopilot 中添加设备](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步骤自行创建。  

5. 上传 .csv 文件，然后选择 " **保存**"。

如果在尝试上传 .csv 文件时收到错误消息，请检查该文件的格式。 可以仅使用硬件哈希，也可使用 OEM 名称、序列号和型号（按列顺序），还可使用 Windows 产品 ID。 你还可以使用 " **添加设备** " 下的链接中提供的示例 .csv 文件来创建设备列表。

.Csv 文件应如下所示：

> **设备序列号、Windows 产品 ID、硬件哈希、制造商名称、设备型号**

> **{serialNumber},,, Microsoft Corporation，Surface 便携机**

>[!NOTE]
> "制造商名称" 和 "设备型号" 区分大小写。

如果不知道为"制造商名称"和"设备型号"设置什么值，可以在设备上运行此代码以收集正确的值：

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 解除

### <a name="important-information"></a>重要信息

Windows Autopilot允许你在为客户管理的设备上配置 Windows 的自定义安装。 如果客户授权这样做，可以取消或隐藏在设置 Windows 时通常呈现给用户的某些设置屏幕，包括"EULA (最终用户许可协议") 接受屏幕。

使用此函数即表示你同意禁止或隐藏旨在为用户提供通知或接受条款的任何屏幕意味着你已获得客户的足够许可和授权来隐藏条款，并且你代表你的客户 (无论组织还是个人用户（在这种情况下) 都同意任何通知并接受适用于你的客户的任何条款。 这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。 如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。