---
title: 利用 Windows Autopilot 简化设备设置 | 合作伙伴中心
description: 利用 Windows AutoPilot 在合作伙伴中心内添加 Windows AutoPilot 部署配置文件以简化设备设置
author: KPacquer
keywords: autopilot, windows autopilot, microsoft autopilot, 零接触部署, oobe, 登录屏幕
ms.localizationpriority: medium
ms.openlocfilehash: b9fc13accd5d229f66ed425ace68e0df00e14016
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877577"
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>利用 Windows Autopilot 简化设备设置 

Windows Autopilot 可在首次启动时简化和保护新 Windows 10 专业版设备的设备设置，而这只需几个步骤即可实现。 若要了解详细信息，请参阅 [Windows AutoPilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)。

## <a name="features"></a>功能

*  对设置设备的最终用户**禁用本地管理员权限**
*  **显示组织的登录页面**。 组织可以预定义登录页面，以将设备添加为工作设备，并使用 Azure Active Directory 加入设备。
*  在 OOBE 完成后，**将设备注册到 Mobile Device Manager (MDM) 中**，例如 Microsoft Intune。
*  利用 Windows AutoPilot 部署配置文件，**简化全新安装体验 (OOBE)**，以仅使用所需的步骤和决策。 

## <a name="requirements"></a>要求

*  设备预安装 Windows 10 专业版创意者更新（1703 或更高版本）或支持高级 PC 的 Windows 10 专业版。
*  称为硬件哈希值（128 HWH 或 4k HWH）的设备标识符，这通常由 OEM 提供。 你将使用标识符分配合作伙伴仪表板内的组织简介。 
*  设备必须可访问 Internet。 设备如果无法连接，则显示默认的 Windows 全新安装体验 (OOBE) 屏幕。
*  将设备注册到 MDM 需要 Azure Active Directory Premium。

## <a name="add-organization-login-pages-to-oobe"></a>向 OOBE 中添加组织登录页面

若要添加特定于组织的页面，请将设备添加到贵组织的 [Azure AD 目录](https://go.microsoft.com/fwlink/?linkid=848958)，并创建登录页面。


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>利用 Windows AutoPilot 部署配置文件从 OOBE 中删除 Windows 页面

**Windows AutoPilot 部署配置文件中的设置示例**
*  在设置中跳过“隐私设置”
*  在设置中禁用本地管理员帐户
*  在设置中自动跳过页面
   *  为工作单位或学校自动选择设置
   *  跳过 Cortana、OneDrive 和 OEM 注册设置页面

### <a name="add-devices-and-apply-a-profile"></a>添加设备和应用配置文件

从你的仪表板，可创建 Windows AutoPilot 部署配置文件，并将其应用于设备列表。

若要配置设备，请上传设备列表，然后创建应用于设备的配置文件并应用它。

1.  添加设备列表。

    销售代理和管理员代理有权将设备列表添加到合作伙伴仪表板内。
    
    间接经销商能够与他们的间接提供商合作添加此列表。

    a.  使用本主题中的 PowerShell 脚本创建 .csv 文件：[Windows AutoPilot 概述](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)。 此 .csv 文件包含设备信息，其中包括序列号、OEM 名称、型号、产品 ID 和设备标识符。 

    b.  在仪表板中，转到**客户** > 选择要接收设备的客户 > **设备 > 添加设备**。

    c.  命名设备的批次，例如“Contoso 销售部门电脑 - 2017 年 4 月订购”。 

    d.  单击**浏览** > 选择设备信息文件 > **验证**。

    **注意：** 如果你尝试上传 .csv 文件后收到一条错误消息，请检查该文件的格式。 8 月之后，你可以仅使用硬件哈希，按该列顺序使用 OEM 名称、序列号和型号，或者使用 Windows 产品 ID。 你还可以使用**添加设备**旁边的链接中提供的示例 .csv 文件。

2.  创建可应用于设备的配置文件。 （只有管理员代理才有权在合作伙伴仪表板内创建并应用配置文件。）

    a.  在**设备**中，单击**添加新的配置文件**。

    b.  命名配置文件，例如“Contoso 桌面配置文件 - 跳过所有 OOBE”。

    c.  配置 OOBE 设置。 例如，检查**在设置中跳过“快速设置”**。

    d.  单击**提交**。

3.  应用配置文件。

    a.  在**设备**的**分配和删除设备**窗格中，选择要配置的设备。 若要选择整个批次，请单击批次名称（例如“Contoso 销售部门电脑 - 2017 年 3 月订购”）旁的复选框。

    b.  单击**应用配置文件**，然后选择相关配置文件（例如“Contoso 桌面配置文件 - 跳过所有 OOBE”)。 设备将在“配置文件”列中显示该配置文件。

4.  可选：通过测试查看你的配置文件是否有效。

    a.  将设备连接到网络，并将其打开。

    b.  验证是否显示相应的 OOBE 屏幕（如果有）。

    c.  若要为新用户准备设备，请完成 OOBE 体验，然后将该设备重置为其出厂默认设置。


## <a name="to-update-or-delete-a-profile"></a>更新或删除配置文件 

将配置文件分配给设备后，可对其进行更新，即使你已将该设备提供给客户。 当设备连接到 Internet 时，它会在 OOBE 过程中下载你的配置文件的最新版本。 如果客户将其设备还原为出厂默认设置，则该设备将重新下载你的配置文件的最新更新。 

### <a name="you-can-remove-a-profile-from-a-device"></a>可从设备中删除配置文件
1. 选择要从其中删除配置文件的设备（或设备的批次）。 

2. 在**分配和删除设备**窗格中，选择**删除配置文件**。

3. 转到要删除的配置文件，然后将其删除。 将从所有设备中删除该配置文件。

在**设备**中，选择配置文件。 可在此处修改现有的设置。

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Windows Autopilot EULA 解除 - 重要信息

使用此工具，你可以在为客户管理的设备上配置 Windows 的单个安装。 如果客户授权你进行此操作，你可以选择不显示或隐藏在设置 Windows 时向用户正常显示的某些设置屏幕，包括 EULA 接受屏幕。 

使用此功能，即表明你同意不显示或隐藏专为用户提供通知或条款接受的任何屏幕，意味着你已从客户方获得隐藏条款的充分许可和授权，并且你已代表你的客户（组织或单个用户，根据具体情况而定）同意所有通知并接受所有对该客户适用的条款。 这包括你同意在不使用此工具禁止显示或隐藏时将向用户呈现的许可证的条款和条件或通知。 如果你的客户尚未从 Microsoft 或其许可的分销商处获取有效的软件许可，则该客户不得在这些设备上使用该 Windows 软件。


