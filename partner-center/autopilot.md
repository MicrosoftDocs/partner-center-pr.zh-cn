---
title: 自定义设备使用 Windows Autopilot 配置文件的全新体验 |合作伙伴中心
description: 使用 Autopilot 配置文件预配置设备的全新体验。
ms.topic: article
ms.date: 03/18/2019
author: maggiepuccievans
ms.author: evansma
keywords: autopilot, windows autopilot, microsoft autopilot, 零接触部署, oobe, 登录屏幕, 现成
ms.localizationpriority: medium
ms.openlocfilehash: 213ed9e45e0109eaa88d7575249272ba403dfcfd
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708744"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>自定义设备的现成体验和 Windows Autopilot 配置文件

**适用于**

- CSP 直接帐单合作伙伴、间接提供商和间接经销商

如果你管理客户设备, 你可能需要为客户的用户自定义全新体验 (OOBE)。 在将设备交付给客户并将新的配置文件应用于客户已购买的设备之前, 可以使用 Windows Autopilot 配置文件预先配置新设备。 

请注意, Oem 已开始在显示设备的**产品密钥 ID (PKID)** 的 Autopilot 设备框之外添加发货标签。  这一维的可读条形码为下游合作伙伴提供了一种方法, 用于为 Autopilot 注册设备, 无需取消装箱设备并通过替代方法获取设备 ID。

本文介绍如何创建 Autopilot 配置文件并将其应用于合作伙伴中心的设备。

如果你尚不熟悉 Autopilot, 请查看以下文章中的信息:

- [Windows Autopilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 部署参考指南](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概述

使用合作伙伴中心的 Windows Autopilot 功能, 你可以创建自定义配置文件以应用于客户设备。 以下配置文件设置在本文发布时可用:

- 跳过隐私设置。 此可选的 Autopilot 配置文件设置使组织无在 OOBE 过程中询问隐私设置。

- 禁用设备上的本地管理员帐户创建。 组织可决定在完成该过程后, 设置设备的用户是否应具有管理员访问权限。

- 为工作或学校自动设置设备。 注册到 Autopilot 的所有设备将自动被视为工作或学校设备, 因此不会在 OOBE 过程中询问此问题。

- 跳过 Cortana、OneDrive 和 OEM 注册设置页。 注册到 Autopilot 的所有设备都会在全新体验 (OOBE) 过程中自动跳过这些页面。

- 跳过最终用户许可协议 (EULA)。 从 Windows 10 版本1709开始, 组织可以决定跳过 OOBE 过程中显示的 EULA 页面。 请参阅下面的[Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal), 以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。

以下配置文件和设备管理权限和限制适用:

- 即使客户已删除合作伙伴的委派管理权限, CSP 合作伙伴也可以继续管理与其拥有分销商关系的现有客户的 Autopilot 配置文件。

- 你可以管理已添加的客户的现有设备。

- 你无法管理客户已上传到 Microsoft Store for Business 或 Microsoft Intune 门户的设备。

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>在合作伙伴中心创建和管理 Autopilot 配置文件

在合作伙伴中心, 你可以创建 Windows Autopilot 部署配置文件并将它们应用到设备。

>[!NOTE]
>只有管理代理可以创建和应用配置文件。

### <a name="create-a-new-autopilot-profile"></a>创建新的 Autopilot 配置文件

1. 从 "合作伙伴中心" 菜单中选择 "**客户**", 然后选择要为其创建 Autopilot 配置文件的客户。

2. 在客户的详细信息页上, 选择 "**设备**"。

3. 在 " **Windows Autopilot 配置文件**" 下, 选择 "**添加新配置文件**"。

4. 输入配置文件的 "名称" 和 "说明", 然后配置 "OOBE" 设置。 选择:  

   - 在安装程序中跳过隐私设置

   - 在设置中禁用本地管理员帐户
  
   - 在设置中自动跳过页面<br>
        (包括*自动选择适用于工作或学校的设置*, 并*跳过 Cortana、OneDrive 和 OEM 注册设置页*)
  
   - 跳过最终用户许可协议 (EULA)<br> 
       >[!IMPORTANT] 
       >请参阅下面的[Windows AUTOPILOT EULA 消除](#windows-autopilot-eula-dismissal), 以了解有关在 Windows 安装过程中跳过 EULA 页面的重要信息。

5. 完成后选择**提交**。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>将 Autopilot 配置文件应用到客户设备

>[!NOTE]
>以下说明假定您已将客户的设备添加到合作伙伴中心, 并且您可以访问其设备列表。 如果尚未添加客户的设备, 请按照[将设备添加到客户帐户](#add-devices-to-a-customers-account)中的说明操作, 然后执行以下步骤。

为客户创建 Autopilot 配置文件后, 可将其应用到客户的设备。

1. 从 "合作伙伴中心" 菜单中选择 "**客户**", 然后选择为其创建 Autopilot 配置文件的客户。

2. 在客户的详细信息页上, 选择 "**设备**"。

3. 在 "**将配置文件应用到设备**" 下, 选择要将配置文件添加到的设备或设备组, 然后选择 "**应用配置文件**"。 刚才应用的配置文件将显示在 "**配置文件**" 列中。

4. 按照以下步骤验证配置文件是否将成功应用到设备。

    a.  将设备连接到网络并将其打开。

    b.  验证是否显示相应的 OOBE 屏幕（如果有）。

    c.  当 OOBE 进程停止时, 将设备重置为其出厂默认设置, 以便为新用户准备。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>从客户的设备中删除 Autopilot 配置文件

1. 从 "合作伙伴中心" 菜单中选择 "**客户**", 然后选择为其创建 Autopilot 配置文件的客户。

2. 在客户的详细信息页上, 选择 "**设备**"。

3. 在 "**将配置文件应用到设备**" 下, 选择要从中删除配置文件的设备, 然后选择 "**删除配置文件**"。

   >[!NOTE]
   >从设备删除配置文件不会从列表中删除该配置文件。 如果要删除配置文件, 请按照[更新或删除 Autopilot 配置文件](#update-or-delete-an-autopilot-profile)中的说明进行操作。

### <a name="update-or-delete-an-autopilot-profile"></a>更新或删除 Autopilot 配置文件

如果客户想要在将设备寄送到设备后更改全新体验, 可以在合作伙伴中心更改该配置文件。

当客户的设备连接到 internet 时, 它将在 OOBE 过程中下载最新的配置文件版本。 此外, 在任何时候, 如果客户将设备恢复为其出厂默认设置, 则设备将在 OOBE 过程中再次下载最新的配置文件版本。

1. 从 "合作伙伴中心" 菜单中选择 "**客户**", 然后选择要更改 Autopilot 配置文件的客户。

2. 在客户的详细信息页上, 选择 "**设备**"。

3. 在 " **Windows Autopilot 配置文件**" 下, 选择需要更新的配置文件。 进行所需的更改, 然后选择 "**提交**"。

若要删除此配置文件, 请选择页面右上角的 "**删除配置文件**"。

### <a name="add-devices-to-a-customers-account"></a>向客户帐户添加设备

>[!NOTE]
>销售代理和管理代理可以将设备添加到客户的帐户。

你必须能够访问客户的设备列表, 然后才能将自定义 Autopilot 配置文件应用到客户设备。

如果计划使用 OEM 名称、序列号和型号组合, 请注意以下限制:

- 此元组仅适用于较新的设备 (例如4k 哈希), 不支持128b 哈希 (RS2 和之前的设备)。

- 元组注册区分大小写, 因此文件中的数据必须与 OEM 提供商 (硬件提供商) 提供的名称***完全***匹配。

按照以下说明将设备添加到合作伙伴中心的客户帐户。

1. 从 "合作伙伴中心" 菜单中选择 "**客户**", 然后选择要管理其设备的客户。

2. 在客户的详细信息页上, 选择 "**设备**"。

3. 在 "**将配置文件应用到设备**" 下选择 "**添加设备**"。

4. 输入 "设备列表" 的名称, 然后选择 "**浏览**" 以将客户列表 (采用 .csv 文件格式) 上传到合作伙伴中心。

    >[!NOTE]
    >你应收到此 .csv 文件, 并购买你的设备。 如果未收到 .csv 文件, 则可以按照[向 Windows Autopilot 中添加设备](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步骤自行创建。  

5. 上传 .csv 文件, 然后选择 "**保存**"。

如果在尝试上传 .csv 文件时收到错误消息, 请检查该文件的格式。 您可以仅使用硬件哈希, 或使用 OEM 名称、序列号和型号 (列顺序) 或 Windows 产品 ID。 你还可以使用 "**添加设备**" 下的链接中提供的示例 .csv 文件来创建设备列表。

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 消除

### <a name="important-information"></a>重要信息

Windows Autopilot 允许你在为客户管理的设备上配置 Windows 的自定义安装。 如果客户有权执行此操作, 则可以禁止或隐藏在设置 Windows 时通常向用户显示的某些安装屏幕, 包括 EULA (最终用户许可协议) 接受屏幕。

通过使用此功能, 即表示你同意禁止或隐藏旨在向用户提供通知或接受条款的任何屏幕, 这意味着你已获得足够的许可和授权, 可供你的客户隐藏条款, 并代表你的客户 (无论是组织还是单个用户作为案例), 同意通知并接受适用于你的客户的任何条款。 这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。 如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。
