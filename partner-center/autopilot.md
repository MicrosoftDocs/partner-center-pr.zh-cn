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
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134707"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>自定义设备的开箱体验与 Windows Autopilot 配置文件

**适用于**

- CSP 直接帐单合作伙伴、 间接提供商和间接经销商

如果您管理客户的设备，你可能需要自定义客户的用户的开箱体验 (OOBE)。 可以将新设备使用 Windows Autopilot 配置文件预配置设备交付给客户之前，并将新的配置文件应用到客户已购买的设备。 此文章介绍了如何创建并应用到合作伙伴中心中的设备的 Autopilot 配置文件。

如果您是不熟悉 Autopilot，查看以下文章中的信息：

- [Windows Autopilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 部署参考指南](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概述

使用合作伙伴中心中的 Windows Autopilot 功能，可以创建自定义配置文件，以适用于客户的设备。 在本文发布的时，以下配置文件设置已可用：

- 跳过的隐私设置。 此可选的 Autopilot 配置文件设置使组织能够在 OOBE 过程不询问有关隐私设置。

- 禁用设备上创建的本地管理员帐户。 组织可以决定是否过程完成后，设置设备的用户应具有管理员访问权限。

- 自动设置为工作或学校帐户的设备。 Autopilot 注册的所有设备将自动被视为工作或学校的设备，因此不会在 OOBE 过程要求这一问题。

- 跳过 Cortana、 OneDrive 和 OEM 注册设置页。 Autopilot 注册的所有设备将在开箱体验 (OOBE) 过程中自动跳都过这些页。

- 跳过最终用户许可协议 (EULA)。 从 Windows 10 1709年版开始，组织可以决定跳过的 OOBE 过程显示 EULA 页面。 请参阅[Windows Autopilot EULA 上诉](#windows-autopilot-eula-dismissal)下面有关在 Windows 过程中跳过 EULA 页面考虑的重要信息设置。

以下配置文件和设备管理权限和限制适用：

- CSP 合作伙伴可以继续为现有的客户必须与其分销商关系管理 Autopilot 配置文件，即使客户已删除的合作伙伴委派的管理权限。

- 为已添加的客户，可以管理现有的设备。

- 不能管理你的客户已上传到 Microsoft Store for Business 或 Microsoft Intune 门户的设备。

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>创建和管理合作伙伴中心中的 Autopilot 配置文件

在合作伙伴中心，可以创建 Windows Autopilot 部署配置文件并将其应用到设备。

>[!NOTE]
>仅管理代理可以创建并应用配置文件。

### <a name="create-a-new-autopilot-profile"></a>创建新的 Autopilot 配置文件

1. 选择**客户**从合作伙伴中心菜单，然后选择客户要创建的 Autopilot 配置文件。

2. 在客户的详细信息页上，选择**设备**。

3. 下**Windows Autopilot 配置文件**选择**添加新的配置文件**。

4. 输入配置文件的名称和描述，然后配置 OOBE 设置。 从选择：  

   - 跳过安装程序中的隐私设置

   - 在设置中禁用本地管理员帐户
  
   - 在设置中自动跳过页面<br>
        (包括*自动选择安装程序的工作或学校*并*跳过 Cortana、 OneDrive 和 OEM 注册设置页*)
  
   - 跳过最终用户许可协议 (EULA)<br> 
       >[!IMPORTANT] 
       >请参阅[Windows Autopilot EULA 上诉](#windows-autopilot-eula-dismissal)下面有关在 Windows 过程中跳过 EULA 页面考虑的重要信息设置。

5. 完成后选择**提交**。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>适用于客户的设备的 Autopilot 配置文件

>[!NOTE]
>下面的说明假定你已添加的客户的设备到合作伙伴中心，并且可以访问其设备列表。 如果你尚未添加客户的设备，请按照中的说明[将设备添加到客户的帐户](#add-devices-to-a-customers-account)然后按照以下步骤进行操作。

为客户创建 Autopilot 配置文件后，可以将其应用到客户的设备。

1. 选择**客户**从合作伙伴中心菜单，然后选择你创建客户的 Autopilot 配置文件。

2. 在客户的详细信息页上，选择**设备**。

3. 下**适用于设备的配置文件**选择设备或设备组你想要添加到配置文件，然后选择**配置文件应用**。 您刚刚应用的配置文件中将出现**配置文件**列。

4. 请按照以下步骤来验证该配置文件将会成功应用到设备。

    a.  将设备连接到网络并将其打开。

    b.  验证是否显示相应的 OOBE 屏幕（如果有）。

    c.  当 OOBE 进程停止时，设备重置为出厂默认设置来准备新的用户。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>从客户的设备中删除 Autopilot 配置文件

1. 选择**客户**从合作伙伴中心菜单，然后选择你创建客户的 Autopilot 配置文件。

2. 在客户的详细信息页上，选择**设备**。

3. 下**适用于设备的配置文件**选择你想要删除的配置文件，然后选择的设备**删除配置文件**。

   >[!NOTE]
   >删除设备中的配置文件不会从列表中删除该配置文件。 如果你想要删除配置文件，请按照中的说明[更新或删除 Autopilot 配置文件](#update-or-delete-an-autopilot-profile)。

### <a name="update-or-delete-an-autopilot-profile"></a>更新或删除 Autopilot 配置文件

如果客户想要更改的开箱体验已寄给他们的设备后，可以更改合作伙伴中心中的配置文件。

当客户的设备连接到 internet 时，它将在 OOBE 过程中下载最新的配置文件版本。 此外，任何时间客户将设备还原为其出厂默认设置，设备将再次下载最新的配置文件版本 OOBE 过程。

1. 选择**客户**从合作伙伴中心菜单，然后选择您需要更改 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择**设备**。

3. 下**Windows Autopilot 配置文件**选择需要更新的配置文件。 进行必要的更改，然后选择**提交**。

若要删除此配置文件，请选择**删除配置文件**从页面的右上角。

### <a name="add-devices-to-a-customers-account"></a>将设备添加到客户的帐户

>[!NOTE]
>销售代理和管理代理可以将设备添加到客户的帐户。

可以将自定义 Autopilot 配置文件应用于客户的设备之前，您必须能够访问客户的设备列表。

如果你打算使用 OEM 名称、 序列号和型号组合，请注意这些限制：

- 此元组仅适用于较新的设备 （4 k 哈希值，例如），不支持 128b 哈希 （RS2 和以前的设备）。

- 元组注册是区分大小写，因此文件中的数据必须与匹配的型号和制造商名称***完全***由 OEM 提供程序 （硬件提供程序） 提供。

请按照以下说明将设备添加到合作伙伴中心中的客户的帐户。

1. 选择**客户**从合作伙伴中心菜单，然后选择客户想要管理其设备。

2. 在客户的详细信息页上，选择**设备**。

3. 下**适用于设备的配置文件**选择**添加设备**。

4. 输入设备列表的名称，然后选择**浏览**将上载到合作伙伴中心 （在.csv 文件格式） 的客户的列表。

    >[!NOTE]
    >你应与你的设备购买收到此.csv 文件。 如果未收到的.csv 文件，则可以按照中的步骤创建一个自己[将设备添加到 Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)。  

5. 上传.csv 文件，然后选择**保存**。

如果尝试上传.csv 文件时遇到一条错误消息，检查文件的格式。 可以使用硬件哈希，或 OEM 名称、 序列号和模型 （在此列顺序） 或 Windows 产品 id。 此外可以使用旁边的链接中提供的示例.csv 文件**将设备添加**若要创建的设备列表。

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 上诉

### <a name="important-information"></a>重要信息

Windows Autopilot 可以为客户管理的设备上配置 Windows 的自定义的安装。 如果被授权执行此操作由客户，可以禁止显示或隐藏某些设置 Windows，包括 EULA （最终用户许可协议） 接受屏幕时正常呈现给用户的设置屏幕。

使用此函数，即表示你同意，禁止显示或隐藏旨在向用户提供通知或已从你的客户代表的隐藏条款，并且您，获取足够的许可和授权条款意味着接受任何屏幕客户 （无论组织或单个用户以这种情况可能），同意任何通知，并接受任何条款适用于你的客户。 这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。 如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。