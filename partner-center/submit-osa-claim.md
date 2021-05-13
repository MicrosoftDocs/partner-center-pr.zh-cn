---
title: 创建客户关联
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: 创建客户与 CPOR 申报记录合作伙伴 (模型) 关联。 帮助管理 Dynamics 365 Microsoft 365 &的销售、使用情况和奖励。
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9526a47d0b6d734bde48f403c11fa84d734511c1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856094"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="ae504-104">通过客户和 Dynamics 365 的 CPOR (CPOR) 客户Microsoft 365关联</span><span class="sxs-lookup"><span data-stu-id="ae504-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="ae504-105">**适当角色**：奖励管理员</span><span class="sxs-lookup"><span data-stu-id="ae504-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="ae504-106">2019 年 10 月 1 日，Microsoft 开始使用 申报记录合作伙伴 (CPOR) 模型来管理与 Microsoft 365 和 Dynamics 365 客户的关联，这些关联涉及联机服务咨询 (OSA) 销售、联机服务使用情况 (OSU) -Microsoft 365 和 OSU-Business 应用程序奖励。</span><span class="sxs-lookup"><span data-stu-id="ae504-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="ae504-107">客户关联 (CPOR) 申请仅适用于联机服务咨询 (OSA) 销售、联机服务使用情况 (OSU) -Microsoft 365 和 OSU-Business 应用程序奖励计划。</span><span class="sxs-lookup"><span data-stu-id="ae504-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="ae504-108">如果要为另一个计划（例如 云解决方案提供商、Managed Reseller、Hosting 或 Surface）提交合作申请，请参阅此处概述的 Co-op 声明过程。</span><span class="sxs-lookup"><span data-stu-id="ae504-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider, Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="ae504-109">提交声明时，Microsoft 会进行验证。</span><span class="sxs-lookup"><span data-stu-id="ae504-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="ae504-110">此时，我们可能会要求你提供详细信息。</span><span class="sxs-lookup"><span data-stu-id="ae504-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="ae504-111">我们还将通知客户你的关联请求。</span><span class="sxs-lookup"><span data-stu-id="ae504-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="ae504-112">客户有五个工作日可以选择退出。如果他们不选择退出，则你与此特定租户和工作负荷的关联将是官方的。</span><span class="sxs-lookup"><span data-stu-id="ae504-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="ae504-113">此时，你有权访问客户的使用情况数据。</span><span class="sxs-lookup"><span data-stu-id="ae504-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="ae504-114">需要以下信息才能完成声明：</span><span class="sxs-lookup"><span data-stu-id="ae504-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="ae504-115">进行声明的实体的 **MPN ID**</span><span class="sxs-lookup"><span data-stu-id="ae504-115">The **MPN ID** for your entity that makes the claim</span></span>

- <span data-ttu-id="ae504-116">客户的域名 **查找**[此](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="ae504-116">Customer's **domain name** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="ae504-117">客户的目录 **ID 或\*\*\*\*租户 ID** [查找此 ID](find-ids-and-domain-names.md)</span><span class="sxs-lookup"><span data-stu-id="ae504-117">Customer's **Directory ID** or **Tenant ID** [Find this](find-ids-and-domain-names.md)</span></span>

- <span data-ttu-id="ae504-118">" **解决方案"** 区域，例如Business Applications或Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ae504-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="ae504-119">**已** 执行的活动以及要声明的类型，例如售前、使用情况或收入关联</span><span class="sxs-lookup"><span data-stu-id="ae504-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="ae504-120">客户的联系人 **姓名、** 标题和电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="ae504-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="ae504-121">对于 Dynamics 365，还需要提供客户的技术联系人姓名、标题和电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="ae504-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="ae504-122">自己公司的 **联系人姓名** 和电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="ae504-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="ae504-123">你将为此声明创建 **名称**</span><span class="sxs-lookup"><span data-stu-id="ae504-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="ae504-124">**产品 ()** 或 () 你所申报的工作负荷</span><span class="sxs-lookup"><span data-stu-id="ae504-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="ae504-125">**(PoE) 的执行证明**，如客户签署的工作声明。</span><span class="sxs-lookup"><span data-stu-id="ae504-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="ae504-126">你还可以下载要使用的 PoE 模板。</span><span class="sxs-lookup"><span data-stu-id="ae504-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="ae504-127">仅适用于申报收入关联的合作伙伴： **Dynamics 解决方案卖方名称**、 **客户名称** 和 **ISV 产品/解决方案的名称**。</span><span class="sxs-lookup"><span data-stu-id="ae504-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="ae504-128">还应了解以下要点：</span><span class="sxs-lookup"><span data-stu-id="ae504-128">You should also understand the following points:</span></span>

- <span data-ttu-id="ae504-129">如果现有 Microsoft 365 客户，则需使用此过程重新与想要继续获得 OSU 激励的用户进行关联。</span><span class="sxs-lookup"><span data-stu-id="ae504-129">If you have existing Microsoft 365 customers, you'll need to re-associate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="ae504-130">如果现有与 Dynamics 365 或 Power BI 客户的关联，则这些关联将保持有效，直到其订阅过期。</span><span class="sxs-lookup"><span data-stu-id="ae504-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="ae504-131">一个客户可以具有多个合作伙伴，但每个工作负荷 (适用于 OSA-Sell 和 OSU-Business 应用程序的 OSU-Microsoft 365) 或订阅 (，) 只能与一个合作伙伴关联。</span><span class="sxs-lookup"><span data-stu-id="ae504-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="ae504-132">创建客户关联</span><span class="sxs-lookup"><span data-stu-id="ae504-132">Create a customer association</span></span>

1. <span data-ttu-id="ae504-133">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="ae504-133">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="ae504-134">选择 " **激励** " 选项卡，选择 " **概述**"，然后选择 " **客户关联**"。</span><span class="sxs-lookup"><span data-stu-id="ae504-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="ae504-135">在 "客户关联" 页的顶部，选择 " **+ 客户关联**"。</span><span class="sxs-lookup"><span data-stu-id="ae504-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="ae504-136">选择要与客户关联的合作伙伴位置的 MPN ID，然后添加客户的域名和目录 ID。</span><span class="sxs-lookup"><span data-stu-id="ae504-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="ae504-137">查找此</span><span class="sxs-lookup"><span data-stu-id="ae504-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="ae504-138">选择“继续”。</span><span class="sxs-lookup"><span data-stu-id="ae504-138">Select **Continue**.</span></span>

6. <span data-ttu-id="ae504-139">选择 **解决方案区域** 和 **活动**。</span><span class="sxs-lookup"><span data-stu-id="ae504-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="ae504-140">如果选择 "Business Applications"，请选择 " **使用情况" 和/或 "提前销售**" 或 " **收入关联**"，然后选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="ae504-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="ae504-141">如果选择“收入关联”，系统将提示你输入与下面所列信息稍有不同的信息。</span><span class="sxs-lookup"><span data-stu-id="ae504-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="ae504-142">在 " **关联客户** " 页上输入相应信息，然后选择 " **创建声明**"。</span><span class="sxs-lookup"><span data-stu-id="ae504-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="ae504-143">选择与此客户关联关联的产品 () ，然后选择 " **继续**"。</span><span class="sxs-lookup"><span data-stu-id="ae504-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="ae504-144">填写客户联系信息和你公司的联系信息。</span><span class="sxs-lookup"><span data-stu-id="ae504-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="ae504-145">所有字段都是必填字段。</span><span class="sxs-lookup"><span data-stu-id="ae504-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="ae504-146">如果你的产品是 Dynamics 365，并且你选择的产品有多个订阅用于此特定客户，则还需要输入订阅 ID。</span><span class="sxs-lookup"><span data-stu-id="ae504-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="ae504-147"> (PoE) 提供执行证明。</span><span class="sxs-lookup"><span data-stu-id="ae504-147">Supply your proof of execution (PoE).</span></span> <span data-ttu-id="ae504-148">可以将其拖到框中，浏览找到自己的支持性文档，或通过选择“下载模板”来使用模板。</span><span class="sxs-lookup"><span data-stu-id="ae504-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="ae504-149">根据需要添加并保存注释，然后选择“提交声明”。</span><span class="sxs-lookup"><span data-stu-id="ae504-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="ae504-150">我们将向客户发送一封电子邮件，请求批准客户关联。</span><span class="sxs-lookup"><span data-stu-id="ae504-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="ae504-151">提交客户关联后，不能对其进行编辑。</span><span class="sxs-lookup"><span data-stu-id="ae504-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="ae504-152">客户关联的状态显示在“状态”字段中。</span><span class="sxs-lookup"><span data-stu-id="ae504-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="ae504-153">选择“历史记录”查看客户关联的历史记录。</span><span class="sxs-lookup"><span data-stu-id="ae504-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ae504-154">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ae504-154">Next steps</span></span>

- [<span data-ttu-id="ae504-155">管理客户关联</span><span class="sxs-lookup"><span data-stu-id="ae504-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)