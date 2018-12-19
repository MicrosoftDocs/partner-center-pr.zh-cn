---
title: 自定义设备的现成的体验的 Windows Autopilot 配置文件 |合作伙伴中心
description: 预配置的 Autopilot 配置文件的设备的现成的体验。
author: maggiepuccievans
keywords: autopilot，windows autopilot、 microsoft autopilot，零接触部署，oobe，登录屏幕，现成的
ms.localizationpriority: medium
ms.openlocfilehash: 7df979042799954c5b43a2adef1915941db02e57
ms.sourcegitcommit: 90d656ed3a4d056a0506f7b5e2b1b8c728f58c46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2018
ms.locfileid: "8976804"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>自定义的 Windows Autopilot 配置文件的设备的现成的体验

**适用范围**

- 云解决方案提供商直接帐单合作伙伴，间接提供商和间接经销商

如果你管理客户的设备，你可能需要自定义的全新体验 (OOBE) 的客户的用户。 你可以交付给客户的设备之前预配置新设备的 Windows Autopilot 配置文件，并将新的配置文件应用到客户已购买的设备。 本文介绍了如何创建 Autopilot 配置文件并应用到合作伙伴中心中的设备。

如果你还不熟悉使用 Autopilot，查看这些文章中的信息：

- [Windows Autopilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Autopilot 部署参考指南](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>概述

与合作伙伴中心中的 Windows Autopilot 功能，你可以创建用于适用于客户设备的自定义配置文件。 在本文发表的时，以下配置文件设置都不可用：

- 跳过隐私设置。 此可选的 Autopilot 配置文件设置可让组织在 OOBE 过程中不询问有关隐私设置。

- 禁用在设备上的创建本地管理员帐户。 组织可以决定是否过程完成后，设置设备的用户应拥有管理员访问权限。

- 自动设置为工作单位或学校的设备。 使用 Autopilot 注册的所有设备自动将被视为工作或学校的设备，因此不会在 OOBE 过程中要求此问题。

- 跳过 Cortana、 OneDrive 和 OEM 注册设置页面。 使用 Autopilot 注册的所有设备将在外的全新体验 (OOBE) 过程中自动跳都过这些页面。

- 跳过最终用户许可协议 (EULA)。 从 Windows 10 版本 1709年开始，组织可以决定跳过 EULA 页在 OOBE 过程中显示。 请参阅[Windows Autopilot EULA 解除](#windows-autopilot-eula-dismissal)下面的重要信息要考虑在 Windows 安装程序期间跳过 EULA 页。

以下配置文件和设备管理权限和限制应用：

- 云解决方案提供商合作伙伴可以继续与其它们具有经销商关系的现有客户管理 Autopilot 配置文件，即使客户已删除合作伙伴的委派的管理权限。

- 你可以为你已由你或其他云解决方案提供商合作伙伴的客户管理现有设备。

- 不能管理客户已上传到适用于企业的 Microsoft Store 或 Microsoft Intune 门户的设备。

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>创建和管理合作伙伴中心中的 Autopilot 配置文件

在合作伙伴中心中，你可以创建 Windows Autopilot 部署配置文件，并将它们应用到设备。

>[!NOTE]
>只有管理员代理可以创建并应用配置文件。

### <a name="create-a-new-autopilot-profile"></a>创建新的 Autopilot 配置文件

1. 从合作伙伴中心菜单中选择**客户**，然后选择你要创建的 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择**设备**。

3. 在**Windows Autopilot 配置文件**中，选择**添加新配置文件**。

4. 输入配置文件的名称和描述，然后配置 OOBE 设置。 从选择：  

   - 在设置中跳过隐私设置
   
   - 在设置中禁用本地管理员帐户
   
   - 在设置中自动跳过页面<br>
        （包括*为工作单位或学校自动选择设置*和*跳过 Cortana、 OneDrive 和 OEM 注册设置页面*）
   
   - 跳过最终用户许可协议 (EULA)<br> 
       >[!IMPORTANT] 请参阅[Windows Autopilot EULA 解除](#windows-autopilot-eula-dismissal)下面的重要信息要考虑在 Windows 安装程序期间跳过 EULA 页。

5. 完成后选择**提交**。

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>适用于客户设备的 Autopilot 配置文件

>[!NOTE]
>以下说明假设，已经向合作伙伴中心添加客户的设备和可以访问其设备列表。 如果你尚未添加客户的设备，按照[将设备添加到客户帐户](#add-devices-to-a-customers-account)中的说明，然后按照下面的步骤。

为客户创建 Autopilot 配置文件后，你可以将其应用到客户的设备。

1. 从合作伙伴中心菜单中选择**客户**，然后选择你创建的 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择**设备**。

3. 在**应用到设备的配置文件**中，选择设备或你想要添加到配置文件，然后选择**应用配置文件**的设备组。 只是应用的配置文件将显示在**配置文件**列中。

4. 请按照以下步骤来验证配置文件将会成功应用到设备。

    a.  将设备连接到网络，并将其打开。

    b.  验证是否显示相应的 OOBE 屏幕（如果有）。

    c.  在 OOBE 过程停止时，设备重置为出厂默认设置为新用户准备它。

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>从客户的设备中删除 Autopilot 配置文件

1. 从合作伙伴中心菜单中选择**客户**，然后选择你创建的 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择**设备**。

3. 在**应用到设备的配置文件**中，选择你想要删除的配置文件，然后选择**删除配置文件**的设备。

  >[!NOTE]
  >从设备中删除配置文件不会从列表中删除配置文件。 如果你想要删除配置文件，请按照[更新或删除 Autopilot 配置文件](#update-or-delete-an-autopilot-profile)中的说明。

### <a name="update-or-delete-an-autopilot-profile"></a>更新或删除 Autopilot 配置文件

如果客户想要更改的现成体验后已交付给他们的设备，你可以更改合作伙伴中心中的配置文件。

当客户的设备连接到 internet 时，它将在 OOBE 过程中下载最新的配置文件版本。 此外，的只要客户将设备还原为出厂默认设置，设备将重新下载最新的配置文件版本在 OOBE 过程中。

1. 从合作伙伴中心菜单中选择**客户**，然后选择想要更改 Autopilot 配置文件的客户。

2. 在客户的详细信息页上，选择**设备**。

3. 在**Windows Autopilot 配置文件**中，选择你需要更新的配置文件。 进行所需的更改，然后选择**提交**。

若要删除该配置文件，从该页面的右上角选择**删除配置文件**。

### <a name="add-devices-to-a-customers-account"></a>将设备添加到客户帐户

>[!NOTE]
>销售代理和管理员代理可以将设备添加到客户帐户。

你可以将自定义的 Autopilot 配置文件应用于客户设备之前，你必须能够访问客户的设备列表。

如果你打算使用的 OEM 名称、 序列号和型号组合，请注意以下限制：

- 此元组仅适用于的较新的设备 （4 k 哈希值，例如），并且不受支持 128b 哈希 （RS2 和之前的设备）。

- 元组注册是区分大小写，因此文件中的数据必须模型和制造商的名称***完全***匹配，因为由 OEM 提供程序 （硬件提供程序） 提供。

请按照以下说明将设备添加到合作伙伴中心中的客户的帐户。

1. 从合作伙伴中心菜单中选择**客户**，然后选择客户想要管理其设备。

2. 在客户的详细信息页上，选择**设备**。

3. 在**应用到设备的配置文件**中，选择**添加设备**。

4. 输入设备列表的名称，然后选择**浏览**要上传到合作伙伴中心的客户的列表 （在.csv 文件格式）。

    >[!NOTE]
    >你应该使用设备购买收到此.csv 文件。 如果你未收到.csv 文件，你可以按照[添加 Windows Autopilot 设备](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)中的步骤来创建自己。  

5. 上传.csv 文件，然后选择**保存**。

如果你尝试上传.csv 文件时收到一条错误消息，请检查文件的格式。 你可以使用硬件哈希，或 OEM 名称、 序列号和模型 （在该列顺序） 或 Windows 产品 id。 你还可以使用**添加设备**旁边的链接中提供的示例.csv 文件创建设备列表。

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA 解除的信息

### <a name="important-information"></a>重要信息

Windows Autopilot 让你可以为你的客户管理的设备上配置 Windows 的自定义的安装。 如果执行此操作由授权客户，你可以禁止显示或隐藏设置 Windows，包括 EULA （最终用户许可协议） 接受屏幕时向用户正常显示的某些设置屏幕。

通过使用此函数，表明你同意禁止显示或隐藏专为用户提供通知或条款接受的术语意味着你已获取足够许可和授权从你的客户可代表隐藏条款，并且该，任何屏幕你的客户 （组织或单个用户以这种情况可能），同意所有通知并接受所有适用于你的客户的条款。 这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。 如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。