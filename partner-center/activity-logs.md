---
title: 通过客户活动日志获取见解
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 了解如何查看和导出活动日志，以深入了解客户帐户事务和其他与客户相关的合作伙伴管理活动。
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1bb98dd71c9e46914b90d5efbfe14404d08275f9
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150584"
---
# <a name="view-or-export-customer-activity-logs-for-more-insight-into-customer-transactions"></a><span data-ttu-id="35aec-103">查看或导出客户活动日志，以更深入地了解客户事务</span><span class="sxs-lookup"><span data-stu-id="35aec-103">View or export customer activity logs for more insight into customer transactions</span></span>

<span data-ttu-id="35aec-104">**适当的角色**：全局管理员|计费管理员|用户管理管理员|管理代理|销售代理|支持人员代理</span><span class="sxs-lookup"><span data-stu-id="35aec-104">**Appropriate roles**: Global admin | Billing admin | User management admin | Admin agent | Sales agent | Helpdesk agent</span></span>

<span data-ttu-id="35aec-105">活动日志为客户提供有关交易和合作伙伴管理操作的信息。</span><span class="sxs-lookup"><span data-stu-id="35aec-105">Activity logs provide information on transactions and Partner management actions for customers.</span></span> <span data-ttu-id="35aec-106">交易日志提供有关交易的详细信息，包括购买的订阅。</span><span class="sxs-lookup"><span data-stu-id="35aec-106">Logs for transactions provide detailed information about the transaction, including purchased subscriptions.</span></span> <span data-ttu-id="35aec-107">还可将活动日志导出为与 Excel 兼容的逗号分隔值文件格式 (.csv)。</span><span class="sxs-lookup"><span data-stu-id="35aec-107">You can also export activity logs to an Excel-compatible comma-separated value file format (.csv).</span></span>

<span data-ttu-id="35aec-108">活动日志提供有关合作伙伴对客户帐户和产品交易所做的操作记录。</span><span class="sxs-lookup"><span data-stu-id="35aec-108">Activity logs provide records for Partner actions on customer accounts and product transactions.</span></span> <span data-ttu-id="35aec-109">还可将活动日志导出到 .csv 文件。</span><span class="sxs-lookup"><span data-stu-id="35aec-109">You can also export activity logs to a .csv file.</span></span>

## <a name="view-and-export-activity-logs"></a><span data-ttu-id="35aec-110">查看和导出活动日志</span><span class="sxs-lookup"><span data-stu-id="35aec-110">View and export activity logs</span></span>

1. <span data-ttu-id="35aec-111">登录到合作伙伴中心[面板](https://partner.microsoft.com/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="35aec-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="35aec-112">从“帐户设置”菜单中，选择“活动日志”。</span><span class="sxs-lookup"><span data-stu-id="35aec-112">From the **Account settings** menu, select **Activity Log**.</span></span>

3. <span data-ttu-id="35aec-113">在“从”和“至”字段中选择活动日志时段。</span><span class="sxs-lookup"><span data-stu-id="35aec-113">Select the activity log period in the **From** and **to** fields.</span></span> <span data-ttu-id="35aec-114">活动日志导出默认定向最近月份。</span><span class="sxs-lookup"><span data-stu-id="35aec-114">The activity log export defaults to the most recent month.</span></span>

   <span data-ttu-id="35aec-115">每个活动日志均提供指向列出客户“订阅”页的链接。</span><span class="sxs-lookup"><span data-stu-id="35aec-115">Each activity log provides a link to the listed customer's **Subscriptions** page.</span></span>

   <span data-ttu-id="35aec-116">选择任意活动日志的向下箭头，查看关于所记录操作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="35aec-116">Select a down arrow for any activity log to view details about a logged action.</span></span> <span data-ttu-id="35aec-117">单个活动日志可显示大量数据，例如多个产品订购。</span><span class="sxs-lookup"><span data-stu-id="35aec-117">A single activity log can show a significant amount of data, such as the ordering of multiple products.</span></span>

4. <span data-ttu-id="35aec-118">日志的数据列包含以下内容：</span><span class="sxs-lookup"><span data-stu-id="35aec-118">The data columns of the log include the following:</span></span>
   - <span data-ttu-id="35aec-119">**日期-时间** - 操作的日期和时间；</span><span class="sxs-lookup"><span data-stu-id="35aec-119">**Date-Time**-the date and time of the action;</span></span>
   - <span data-ttu-id="35aec-120">**受影响的客户** - 客户的公司名称；</span><span class="sxs-lookup"><span data-stu-id="35aec-120">**Affected customer**—the customer's company name;</span></span>
   - <span data-ttu-id="35aec-121">**操作** - 客户执行的操作，例如“创建了一个引荐”；</span><span class="sxs-lookup"><span data-stu-id="35aec-121">**Action**—the action taken by the customer such as "created a referral";</span></span>
   - <span data-ttu-id="35aec-122">**合作伙伴用户** - 与活动关联的合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="35aec-122">**Partner user**—the partner associated with the activity.</span></span>

5. <span data-ttu-id="35aec-123">选择“导出日志”，将客户订阅数据转换为 .csv 文件，并将其下载到计算机上的默认下载文件夹。</span><span class="sxs-lookup"><span data-stu-id="35aec-123">Select **Export log** to copy the customer's subscription data into a .csv file and download it to the default download folder on your computer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="35aec-124">后续步骤</span><span class="sxs-lookup"><span data-stu-id="35aec-124">Next steps</span></span>

- [<span data-ttu-id="35aec-125">分析订阅和许可证以帮助推动业务决策</span><span class="sxs-lookup"><span data-stu-id="35aec-125">Analyze subscriptions and licenses to help drive business decisions</span></span>](analyze-subscriptions-licenses.md)
