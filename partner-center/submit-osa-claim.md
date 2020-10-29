---
title: 创建客户关联
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 创建与申报 (CPOR) 型号的客户关联。 有助于管理 Microsoft 365 & Dynamics 365 客户的销售、使用情况、奖励。
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fec01e6c4554421593de4135ccd1af5c5e7ce13b
ms.sourcegitcommit: 1840767efa4c5de41889bc9245567cf286a084c8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2020
ms.locfileid: "92917241"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="19fd3-104">针对 Microsoft 365 和 Dynamics 365，通过声明的记录 (CPOR) 模型的客户关联</span><span class="sxs-lookup"><span data-stu-id="19fd3-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>

<span data-ttu-id="19fd3-105">**适用于**</span><span class="sxs-lookup"><span data-stu-id="19fd3-105">**Applies to**</span></span>

- <span data-ttu-id="19fd3-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="19fd3-106">Partner Center</span></span>

<span data-ttu-id="19fd3-107">**相应的角色：**</span><span class="sxs-lookup"><span data-stu-id="19fd3-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="19fd3-108">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="19fd3-108">Incentives admin</span></span>

<span data-ttu-id="19fd3-109">2019年10月1日，Microsoft 开始使用 (CPOR) 模型的 "申报合作伙伴" 来管理与 Microsoft 365 和 Dynamics 365 客户相关的关联，和 Dynamics 客户与在线服务顾问联系) ， ("</span><span class="sxs-lookup"><span data-stu-id="19fd3-109">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regards to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="19fd3-110">客户关联 (CPOR) 声明仅适用于在线服务咨询 (OSA) 销售、在线服务使用 (OSU) Microsoft 365 和 OSU-Business 应用程序奖励计划。</span><span class="sxs-lookup"><span data-stu-id="19fd3-110">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="19fd3-111">如果要为其他程序（如云解决方案提供商、托管分销商、托管或 Surface）提交合作声明，请参阅此处所述的合作声明过程。</span><span class="sxs-lookup"><span data-stu-id="19fd3-111">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="19fd3-112">提交声明时，Microsoft 将对其进行验证。</span><span class="sxs-lookup"><span data-stu-id="19fd3-112">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="19fd3-113">此时，我们可能会要求你提供详细信息。</span><span class="sxs-lookup"><span data-stu-id="19fd3-113">We may ask you for more information at this point.</span></span> <span data-ttu-id="19fd3-114">我们还将通知客户你的关联请求。</span><span class="sxs-lookup"><span data-stu-id="19fd3-114">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="19fd3-115">客户需要5个工作日来选择退出。如果未选择退出，则与此特定租户和工作负荷的关联将为官方。</span><span class="sxs-lookup"><span data-stu-id="19fd3-115">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="19fd3-116">此时，你将可以访问客户的使用情况数据。</span><span class="sxs-lookup"><span data-stu-id="19fd3-116">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="19fd3-117">你将需要以下信息来完成声明：</span><span class="sxs-lookup"><span data-stu-id="19fd3-117">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="19fd3-118">构成声明的实体的 **MPN ID**</span><span class="sxs-lookup"><span data-stu-id="19fd3-118">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="19fd3-119">客户的 **域名**[查找此](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="19fd3-119">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="19fd3-120">客户的 **目录 id** 或 **租户 id** [查找此](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="19fd3-120">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="19fd3-121">**解决方案区域** ，如 Business Applications 或 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="19fd3-121">The **Solution area** , such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="19fd3-122">已执行的 **活动** 和要进行的声明的类型，例如售前、使用情况或收入关联</span><span class="sxs-lookup"><span data-stu-id="19fd3-122">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="19fd3-123">你的客户的 **联系人姓名** 、标题和电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="19fd3-123">Your customer's **Contact name** , title, and email address</span></span>

- <span data-ttu-id="19fd3-124">对于 Dynamics 365，还需要提供客户的 **技术联系人** 姓名、职务和电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="19fd3-124">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="19fd3-125">自己公司的 **联系人姓名** 和电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="19fd3-125">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="19fd3-126">你将为此声明创建 **名称**</span><span class="sxs-lookup"><span data-stu-id="19fd3-126">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="19fd3-127">**产品 ()** 或 () 你所申报的工作负荷</span><span class="sxs-lookup"><span data-stu-id="19fd3-127">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="19fd3-128">**(PoE) 的执行证明** ，如客户签署的工作声明。</span><span class="sxs-lookup"><span data-stu-id="19fd3-128">**Proof of execution (PoE)** , such as a statement of work signed by the customer.</span></span> <span data-ttu-id="19fd3-129">你还可以下载要使用的 PoE 模板。</span><span class="sxs-lookup"><span data-stu-id="19fd3-129">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="19fd3-130">仅适用于申报收入关联的合作伙伴： **Dynamics 解决方案卖方名称** 、 **客户名称** 和 **ISV 产品/解决方案的名称** 。</span><span class="sxs-lookup"><span data-stu-id="19fd3-130">For partners claiming revenue association only: **Dynamics solution seller name** , **Customer name** , and **Name of ISV product/solution** .</span></span> 

<span data-ttu-id="19fd3-131">还应了解以下要点：</span><span class="sxs-lookup"><span data-stu-id="19fd3-131">You should also understand the following points:</span></span>

- <span data-ttu-id="19fd3-132">如果现有 Microsoft 365 客户，则需使用此过程重新与想要继续获得 OSU 激励的用户进行关联。</span><span class="sxs-lookup"><span data-stu-id="19fd3-132">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="19fd3-133">如果现有与 Dynamics 365 或 Power BI 客户的关联，则这些关联将保持有效，直到其订阅过期。</span><span class="sxs-lookup"><span data-stu-id="19fd3-133">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="19fd3-134">一个客户可以具有多个合作伙伴，但每个工作负荷 (适用于 OSA-Sell 和 OSU-Business 应用程序的 OSU-Microsoft 365) 或订阅 (，) 只能与一个合作伙伴关联。</span><span class="sxs-lookup"><span data-stu-id="19fd3-134">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="19fd3-135">创建客户关联</span><span class="sxs-lookup"><span data-stu-id="19fd3-135">Create a customer association</span></span>

1. <span data-ttu-id="19fd3-136">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="19fd3-136">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="19fd3-137">选择 " **激励** " 选项卡，选择 " **概述** "，然后选择 " **客户关联** "。</span><span class="sxs-lookup"><span data-stu-id="19fd3-137">Select the **Incentives** tab, select **Overview** , and then select **Customer associations** .</span></span>

3. <span data-ttu-id="19fd3-138">在 "客户关联" 页的顶部，选择 " **+ 客户关联** "。</span><span class="sxs-lookup"><span data-stu-id="19fd3-138">At the top of the Customer associations page, select **+ Customer association** .</span></span>

4. <span data-ttu-id="19fd3-139">选择要与客户关联的合作伙伴位置的 MPN ID，然后添加客户的域名和目录 ID。</span><span class="sxs-lookup"><span data-stu-id="19fd3-139">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="19fd3-140">查找此</span><span class="sxs-lookup"><span data-stu-id="19fd3-140">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="19fd3-141">选择“继续”。</span><span class="sxs-lookup"><span data-stu-id="19fd3-141">Select **Continue** .</span></span>

6. <span data-ttu-id="19fd3-142">选择 **解决方案区域** 和 **活动** 。</span><span class="sxs-lookup"><span data-stu-id="19fd3-142">Select the **Solution area** and **Activity** .</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="19fd3-143">如果选择 "Business Applications"，请选择 " **使用情况" 和/或 "提前销售** " 或 " **收入关联** "，然后选择 " **继续** "。</span><span class="sxs-lookup"><span data-stu-id="19fd3-143">If you select Business Applications, select either **Usage and/or Pre-sales** , or **Revenue association** , and then select **Continue** .</span></span> 
   <br><br><span data-ttu-id="19fd3-144">如果选择“收入关联”，系统将提示你输入与下面所列信息稍有不同的信息。</span><span class="sxs-lookup"><span data-stu-id="19fd3-144">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="19fd3-145">在 " **关联客户** " 页上输入相应信息，然后选择 " **创建声明** "。</span><span class="sxs-lookup"><span data-stu-id="19fd3-145">Enter the appropriate information on the **Associate customer** page, and then select **Create claim** .</span></span>

8. <span data-ttu-id="19fd3-146">选择与此客户关联关联的产品 () ，然后选择 " **继续** "。</span><span class="sxs-lookup"><span data-stu-id="19fd3-146">Select the product(s) associated with this customer association, and then select **Continue** .</span></span>

9. <span data-ttu-id="19fd3-147">填写客户联系信息和你公司的联系信息。</span><span class="sxs-lookup"><span data-stu-id="19fd3-147">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="19fd3-148">所有字段都是必填字段。</span><span class="sxs-lookup"><span data-stu-id="19fd3-148">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="19fd3-149">如果你的产品是 Dynamics 365，并且你选择的产品有多个订阅用于此特定客户，则还需要输入订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="19fd3-149">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="19fd3-150"> (PoE) 提供执行证明。</span><span class="sxs-lookup"><span data-stu-id="19fd3-150">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="19fd3-151">可以将其拖到框中，浏览找到自己的支持性文档，或通过选择“下载模板”来使用模板。</span><span class="sxs-lookup"><span data-stu-id="19fd3-151">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template** .</span></span> 

11. <span data-ttu-id="19fd3-152">根据需要添加并保存注释，然后选择“提交声明”。</span><span class="sxs-lookup"><span data-stu-id="19fd3-152">Add and save comments if you like, and then select **Submit claim** .</span></span> <span data-ttu-id="19fd3-153">我们将向客户发送一封电子邮件，请求批准客户关联。</span><span class="sxs-lookup"><span data-stu-id="19fd3-153">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="19fd3-154">提交客户关联后，不能对其进行编辑。</span><span class="sxs-lookup"><span data-stu-id="19fd3-154">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="19fd3-155">客户关联的状态显示在“状态”字段中。</span><span class="sxs-lookup"><span data-stu-id="19fd3-155">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="19fd3-156">选择“历史记录”查看客户关联的历史记录。</span><span class="sxs-lookup"><span data-stu-id="19fd3-156">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="19fd3-157">后续步骤</span><span class="sxs-lookup"><span data-stu-id="19fd3-157">Next steps</span></span>

- [<span data-ttu-id="19fd3-158">管理客户关联</span><span class="sxs-lookup"><span data-stu-id="19fd3-158">Manage customer associations</span></span>](incentives-manage-customer-associations.md)