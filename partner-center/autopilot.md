---
title: "利用 Windows Autopilot 添加零接触部署配置文件以简化设备设置 | 合作伙伴中心"
description: "利用 Windows Autopilot 在合作伙伴中心内添加零接触部署配置文件以简化设备设置"
author: KPacquer
keywords: "autopilot, windows autopilot, microsoft autopilot, ztd, 零接触部署, oobe, 登录屏幕"
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: c51d9204b352b548a4095e96944aacdbcde97fa2
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2017
---
# <a name="add-a-zero-touch-deployment-profile-to-simplify-device-setup-with-windows-autopilot"></a>利用 Windows Autopilot 添加零接触部署配置文件以简化设备设置

Windows Autopilot 可在首次启动时简化和保护新 Windows 10 专业版设备的设备设置，而这只需几个步骤即可实现。 

## <a name="features"></a>功能

*  对设置设备的最终用户**禁用本地管理员权限**
*  **显示组织的登录页面**。 组织可以预定义登录页面，以将设备添加为工作设备，并使用 Azure Active Directory 加入设备。
*  在 OOBE 完成后，**将设备注册到 MDM 中**，例如 Microsoft Intune。
*  利用零接触部署 (ZTD) 配置文件，**简化全新安装体验 (OOBE)**，以仅使用所需的步骤和决策。 

## <a name="requirements"></a>要求

*  设备预安装 Windows 10 专业版创意者更新（1703 或更高版本）
*  称为硬件哈希值（128 HWH 或 4k HWH）的设备标识符，这通常由 OEM 提供。 你将使用标识符分配合作伙伴中心内的组织配置文件。
*  设备必须可访问 Internet。 设备如果无法连接，则显示默认的 Windows 全新安装体验 (OOBE) 屏幕。
*  将设备注册到 MDM 需要 Azure Active Directory Premium。

## <a name="add-organization-login-pages-to-oobe"></a>向 OOBE 中添加组织登录页面

若要添加特定于组织的页面，请将设备添加到贵组织的 [Azure AD 目录](https://go.microsoft.com/fwlink/?linkid=848958)，并创建登录页面。


## <a name="remove--windows-pages-from-oobe-with-a-zero-touch-deployment-ztd-profile"></a>利用零接触部署 (ZTD) 配置文件从 OOBE 中删除 Windows 页面

### <a name="examples-of-settings-in-a-ztd-profile"></a>ZTD 配置文件中的设置示例
*  在设置中跳过“隐私设置”
*  在设置中禁用本地管理员帐户
*  在设置中自动跳过页面
   *  为工作单位或学校自动选择设置
   *  跳过 Cortana、OneDrive 和 OEM 注册设置页面

### <a name="add-devices-and-apply-a-profile"></a>添加设备和应用配置文件

在合作伙伴中心内，可创建 ZTD 配置文件，并将其应用于设备列表。

若要配置设备，请将设备列表上传到合作伙伴中心，然后创建应用于设备的配置文件并应用它。

1.  将设备列表添加到合作伙伴中心内。 （销售代理和管理员代理有权将设备列表添加到合作伙伴中心内。）

    a.  向 OEM 索要列出新设备的 .csv 文件。 此文件包含序列号和产品 ID，以及通过 OEM Activation 3.0 工具生成的设备标识符。 

    b.  在合作伙伴中心仪表板中，转到**客户** > 选择要接收设备的客户 > **设备 > 添加设备**。

    c.  命名设备的批次，例如“Contoso 销售部门电脑 - 2017 年 4 月订购”。 

    d.  单击**浏览** > 选择设备信息文件 > **验证**。

2.  创建可应用于设备的配置文件。 （只有管理员代理才有权在合作伙伴中心内创建并应用配置文件。）

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

###<a name="you-can-remove-a-profile-from-a-device"></a>可从设备中删除配置文件
1. 选择要从其中删除配置文件的设备（或设备的批次）。 

2. 在**分配和删除设备**窗格中，选择**删除配置文件**。

3. 转到要删除的配置文件，然后将其删除。 将从所有设备中删除该配置文件。


在**设备**中，选择配置文件。 可在此处修改现有的设置。

