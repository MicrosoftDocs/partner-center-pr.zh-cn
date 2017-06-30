---
title: "创建用户帐户和设置权限 | 合作伙伴中心"
description: "管理员为每个需要访问合作伙伴中心的合作伙伴员工创建用户帐户。"
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: 842071dad94251ee498c9dee3e8b689e2e036485
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>创建用户帐户并分配权限

**适用于**

-  合作伙伴中心

为需要访问合作伙伴中心的员工创建用户帐户。 这些任务必须由具有用户管理管理员权限的管理员完成。 

## <a name="add-a-new-user"></a>添加新用户

1. 在**仪表板**菜单上，选择**帐户设置 > 用户管理**。

2.  选择**添加用户**。

3.  输入用户全名和唯一的电子邮件地址。

4.  选择代理类型和管理员类型。 合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，以仅显示用户完成特定任务所需的功能。 有关每个角色可以执行哪些操作的详细信息，请参阅[分配用户权限](#assignuserpermissions)。

5.  选择**添加**，创建用户帐户。 在下一页上确认用户的详细信息。

>**重要提示**<br>
记下此页面上显示的新用户的登录信息。 确保复制这些信息并将其发送给新用户，因为你以后无法再次访问该信息。 <br>

>用户将需要使用其用户名和临时密码登录合作伙伴中心。 当用户首次登录到合作伙伴中心时，会提示他们更改密码。    


### <a href="" id="assignuserpermissions"></a>分配用户权限

合作伙伴中心访问权限基于角色，因此你可以分配自定义用户视图的权限，以仅显示用户完成特定任务所需的功能。 

对于每个用户，你必须选择两个权限级别：

-   代理权限控制用户可以查看和更改哪种类型的客户数据和帐户信息。

-   管理员权限控制用户具有的合作伙伴中心功能访问权限级别。 此设置对合作伙伴中心没有影响 - 帐单管理员可以访问所有 Microsoft 服务的帐单（即使与云解决方案提供商无关），并且全局管理员还可以访问用户帐户和云解决方案提供商以外的客户帐户。

>**重要提示** 默认设置应始终为**不是管理员**，除非用户的角色需要其他访问权限来完成任务和支持客户。

下表介绍了每个角色可以在合作伙伴中心执行的操作。

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>合作伙伴中心中的角色</strong></p></td>
<td><p><strong>他们可以执行的操作</strong></p></td>
<td><p><strong>他们不可以执行的操作</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>管理员代理</strong></p></td>
<td><ul>
<li><p>客户管理</p></li>
<li><p>将设备列表添加到合作伙伴中心</p></li>
<p><li>创建配置文件并将其应用于设备</p></li>
<li><p>订阅管理</p></li>
<li><p>客户的服务运行状况和服务请求</p></li>
<li><p>请求委派的管理员权限</p></li>
<li><p>查看定价和产品/服务</p></li>
<li><p>计费</p></li>
<li><p>代表客户进行管理</p></li>
<li><p>注册增值的经销商</p></li>
</ul></td>
<td><ul>
<li><p>用户管理</p></li>
<li><p>合作伙伴中心的服务请求</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>销售代理</strong></p></td>
<td><ul>
<li><p>客户管理</p></li>
<li><p>将设备列表添加到合作伙伴中心</p></li>
<li><p>订阅管理</p></li>
<li><p>查看支持票证</p></li>
<li><p>请求与客户建立关系</p></li>
<li><p>管理潜在客户</p></li>
<li><p>查看客户协议</p></li>
<li><p>注册一个增值的经销商</p></li>
</ul></td>
<td><ul>
<li><p>针对合作伙伴中心问题创建服务请求</p></li>
<li><p>解决支持票证</p></li>
<li><p>查看服务运行状况</p></li>
<li><p>查看定价和产品</p></li>
<li><p>计费</p></li>
<li><p>代表客户进行管理</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>支持人员代理</strong></p></td>
<td><ul>
<li><p>搜索和查看客户</p></li>
<li><p>编辑客户详细信息</p></li>
<li><p>服务运行状况</p></li>
<li><p>代表客户请求支持（请注意：你必须是管理员代理才能完成此 Office 365 订阅任务）</p></li>
<li><p>代表客户管理订阅和服务（请注意：你必须是管理员代理才能完成此 Office 365 订阅任务）</p></li>
</ul></td>
<td><ul>
<li><p>查看合作伙伴配置文件</p></li>
<li><p>创建新客户帐户</p></li>
<li><p>编辑客户计费信息</p></li>
<li><p>管理订阅</p></li>
<li><p>请求与客户建立关系</p></li>
<li><p>管理潜在客户</p></li>
<li><p>查看定价和产品</p></li>
<li><p>查看客户协议</p></li>
<li><p>计费</p></li>
<li><p>注册一个增值的经销商</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>全局管理员</strong></p></td>
<td><ul>
<li><p>具有可以访问所有 Microsoft 帐户/服务的完整权限</p></li>
<li><p>创建合作伙伴中心的支持票证</p></li>
<li><p>查看协议、价目表和产品</p></li>
<li><p>计费</p></li>
<li><p>查看、创建和管理合作伙伴用户</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>帐单管理员</strong></p></td>
<td><ul>
<li><p>具有可以访问来自 Microsoft 的所有帐单的完整权限</p></li>
<li><p>查看协议、价目表和产品</p></li>
<li><p>计费</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>用户管理管理员</strong></p></td>
<td><ul>
<li><p>查看、创建和管理用户</p></li>
<li><p>查看所有合作伙伴配置文件</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

 

 

 



