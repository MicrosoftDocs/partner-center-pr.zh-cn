---
title: 确认客户接受 Microsoft 客户协议
description: 了解如何确认客户接受 Microsoft 客户协议。 为客户订购 Microsoft 产品和服务时，可能需要这样做。
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029910"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>确认客户接受 Microsoft 客户协议


**相应的角色**

- 管理员代理
- 销售代理

> [!NOTE]
> 目前，协议资源仅受 Microsoft 公有云中合作伙伴中心的支持。 它不适用于：
> * 由世纪互联运营的合作伙伴中心
> * 德国 Microsoft 云合作伙伴中心
> * Microsoft Cloud for US Government 合作伙伴中心


作为合作伙伴，你需要在为客户订购 Microsoft 产品和服务之前确认该客户接受了 Microsoft 客户协议。 为了更好地帮助合作伙伴满足合规性要求，Microsoft 要求合作伙伴通过提供有关接受协议人员的以下详细信息来确认接受协议：

- 名字

- 姓氏

- 电子邮件地址

- 电话号码（可选）

- 接受日期

直接计费合作伙伴和间接提供商在通过合作伙伴中心或合作伙伴中心 API 进行交易时必须确认客户接受了 Microsoft 客户协议。 “确认”为必选项。 

>[!NOTE]
>从 2020 年 1 月 31 日起，所有客户（无论是现有客户还是新客户）都必须签署新的 Microsoft 客户协议。 若要了解详细信息，请参阅[确认客户接受 Microsoft 客户协议](confirm-customer-agreement.md)。

如果没有为给定客户提供确认：

- 你将无法为此客户创建新订单。

- 你无法为此客户更改现有基于许可证的订阅的许可证计数。

可以通过合作伙伴中心或合作伙伴中心 API 确认客户接受。 若要通过合作伙伴中心 API 执行此操作，请参阅以下主题：

- [获取客户同意的确认](/partner-center/develop/get-confirmation-of-customer-consent)

- [获取协议元数据](/partner-center/develop/get-agreement-metadata)

- [确认客户同意](/partner-center/develop/confirm-customer-consent)

这适用于生产环境和沙盒环境。

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>确认新客户接受了协议

在合作伙伴中心中创建新客户租户时，可使用下面的过程来确认客户接受了协议。 必须是管理员代理或销售代理才能执行此操作。

1. 依次选择“客户”、“新客户”、“帐户信息”。   

2. 输入“公司”和“主要联系人”的信息。  

   :::image type="content" source="images/mca/mca1.png" alt-text="公司信息":::

3. 在“Microsoft 客户协议”下，选择“客户已接受最新的 Microsoft 客户协议”。  

4. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。

5. 输入提供接受的用户的详细信息。

   :::image type="content" source="images/mca/MCA3.png" alt-text="添加接受日期":::

   默认情况下，将显示主要联系人用户信息。 如果此信息不正确，请选择“更新”，然后输入接受协议的人员的“名字”、“姓氏”、“电子邮件地址”和*“电话号码”（可选）。     

6. 选择“下一步”  ，继续执行创建客户租户的其余步骤。

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>确认现有客户接受了协议

必须是管理员代理或销售代理才能执行此操作。

1. 选择“客户”，然后找到并选择要查看的客户。

2. 选择“帐户信息”。 

3. 在“Microsoft 客户协议”下，选择“更新”。  

   :::image type="content" source="images/mca/mca4.png" alt-text="Update":::

4. 输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    

5. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。

6. 选择“保存并继续”。 

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>在为现有客户创建新订单时确认客户接受了协议

如果为之前未确认过是否接受了协议的现有客户创建新订单，你将收到完成确认的提示。 请使用下面的过程执行此操作。

1. 输入接受协议的用户的“名字”、“姓氏”、“电子邮件地址”和“电话号码”（可选）。    

2. 在“协议接受日期”  下，输入相应的日期。 不能将此日期设置为未来日期。

3. 选择“保存并继续”。 

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>为现有客户检索客户接受了协议的确认

可以使用下面的过程为之前提供过确认的现有客户检索客户接受了协议的确认。 必须是管理员代理或销售代理才能执行此操作。

1. 选择“客户”，然后找到并选择要查看的客户。

2. 选择“帐户信息”。 

3. 在“Microsoft 客户协议”下，可以看到是否已为此客户提供过确认。 

## <a name="next-steps"></a>后续步骤

- [确认客户接受云解决方案提供商合作伙伴计划中的 Microsoft 客户协议](confirm-customer-agreement.md)

- [代表客户证明接受 Microsoft 客户协议](attest-acceptance-customer-agreement.md)