---
title: 在合作伙伴中心创建和管理付款资料和税务资料
ms.topic: article
ms.date: 06/29/2020
description: 你必须先创建支出和税务配置文件，然后才能支付奖励。
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: kim-davis
ms.author: kimnich
ms.localizationpriority: medium
ms.openlocfilehash: 02212a09ab18ff5b978107af00ac990aa0c702a3
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949683"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="90c57-103">合作伙伴中心的支出和税务配置文件</span><span class="sxs-lookup"><span data-stu-id="90c57-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="90c57-104">适用于：</span><span class="sxs-lookup"><span data-stu-id="90c57-104">Applies to:</span></span>

- <span data-ttu-id="90c57-105">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="90c57-105">Partner Center</span></span>

<span data-ttu-id="90c57-106">必须首先通过将有效的付款和税务配置文件与奖励计划和 MPN 位置相关联来完成注册，然后才能收到针对特定 MPN 位置的奖励计划的付款。</span><span class="sxs-lookup"><span data-stu-id="90c57-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="90c57-107">Microsoft 将使用此付款和税务配置文件来发放款项。</span><span class="sxs-lookup"><span data-stu-id="90c57-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="90c57-108">根据具体的奖励计划规则，你可以使用电子银行转帐或贷方通知单来接收付款。</span><span class="sxs-lookup"><span data-stu-id="90c57-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="90c57-109">适当的角色：</span><span class="sxs-lookup"><span data-stu-id="90c57-109">Appropriate roles:</span></span>

- <span data-ttu-id="90c57-110">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="90c57-110">Incentives admin</span></span>
- <span data-ttu-id="90c57-111">计费管理员</span><span class="sxs-lookup"><span data-stu-id="90c57-111">Billing admin</span></span>
- <span data-ttu-id="90c57-112">全局管理员</span><span class="sxs-lookup"><span data-stu-id="90c57-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="90c57-113">在合作伙伴中心创建和管理付款资料和税务资料</span><span class="sxs-lookup"><span data-stu-id="90c57-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="90c57-114">以下各节将引导你完成在合作伙伴中心创建和管理付款和税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="90c57-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="90c57-115">您必须是激励管理员才能在合作伙伴中心创建或管理付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="90c57-116">奖励角色必须分配给每个激励计划下的每个 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="90c57-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="90c57-117">有关如何在合作伙伴中心添加激励管理员的详细信息，请参阅[如何在合作伙伴中心添加激励用户或管理员](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center)。</span><span class="sxs-lookup"><span data-stu-id="90c57-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="90c57-118">访问合作伙伴中心的支出和税务部分</span><span class="sxs-lookup"><span data-stu-id="90c57-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="90c57-119">使用 AAD 帐户（公司帐户）登录到合作伙伴中心，或使用适当的电子邮件地址（如果已分配）登录。</span><span class="sxs-lookup"><span data-stu-id="90c57-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="90c57-120">可以在一个 AAD 帐户中注册多个域。</span><span class="sxs-lookup"><span data-stu-id="90c57-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="90c57-121">请与全局管理员联系，以确定与哪些域相关联。</span><span class="sxs-lookup"><span data-stu-id="90c57-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="90c57-122">如果只能用 **@onmicrosoft.com** 域登录，请与帐户管理员联系，将其他域添加到 AAD 帐户。</span><span class="sxs-lookup"><span data-stu-id="90c57-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="90c57-123">如果系统提示选择**工作或学校帐户**或**个人帐户**，请选择 "**工作或学校帐户**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="90c57-124">选择齿轮图标以打开 "**设置**" 菜单，然后选择 "**合作伙伴设置**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="90c57-125">在 "**帐户设置**" 菜单中，选择 "**支出和税金**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="90c57-126">将支出和税务配置文件分配给单个计划</span><span class="sxs-lookup"><span data-stu-id="90c57-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="90c57-127">在 "合作伙伴中心"，选择齿轮图标以打开 "**设置**" 菜单。</span><span class="sxs-lookup"><span data-stu-id="90c57-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="90c57-128">选择 "**合作伙伴设置**"，展开 "**支出和税务" 部分**，然后选择 "**分配**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="90c57-129">将显示你的程序列表。</span><span class="sxs-lookup"><span data-stu-id="90c57-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="90c57-130">选择程序旁边的箭头以查看配置文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="90c57-131">在 "**税务配置文件**" 下拉菜单中，选择所需的税务配置文件，或选择 "创建新配置文件" 选项。</span><span class="sxs-lookup"><span data-stu-id="90c57-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="90c57-132">选择用于创建新配置文件的选项时，会相应地重定向。</span><span class="sxs-lookup"><span data-stu-id="90c57-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="90c57-133">在弹出窗口中选择 "继续"。</span><span class="sxs-lookup"><span data-stu-id="90c57-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="90c57-134">下面提供了创建新的税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="90c57-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="90c57-135">选择 "**付款方式**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="90c57-136">如果已选择 "将**电子银行转帐**作为付款方式"，则在 "付款配置文件" 下拉列表中选择所需的付款配置文件，或选择 "创建新配置文件" 选项。</span><span class="sxs-lookup"><span data-stu-id="90c57-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="90c57-137">选择用于创建新配置文件的选项时，会相应地重定向。</span><span class="sxs-lookup"><span data-stu-id="90c57-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="90c57-138">在弹出窗口中选择 "继续"。</span><span class="sxs-lookup"><span data-stu-id="90c57-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="90c57-139">下面提供了创建新付款配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="90c57-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="90c57-140">如果你选择了**贷方通知单**作为付款方法，则完成验证以确认引用的 SAP 编号属于你的组织。</span><span class="sxs-lookup"><span data-stu-id="90c57-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="90c57-141">如果列出了多个 Microsoft 业务实体，则必须为每个实体选择付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="90c57-142">付款方式的可用性取决于激励计划的规则。</span><span class="sxs-lookup"><span data-stu-id="90c57-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="90c57-143">选择**货币**。</span><span class="sxs-lookup"><span data-stu-id="90c57-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="90c57-144">完成所有付款字段后，选择 "**提交**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="90c57-145">创建银行配置文件</span><span class="sxs-lookup"><span data-stu-id="90c57-145">Create your bank profile</span></span>

<span data-ttu-id="90c57-146">银行配置文件是在组织级别创建的，它允许将同一银行配置文件分配到组织内的多个 MPN ID 和激励计划。</span><span class="sxs-lookup"><span data-stu-id="90c57-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="90c57-147">将银行配置文件应用于不同的国家/地区时，可能会出现例外，因为不同的银行和税务规则可能适用。</span><span class="sxs-lookup"><span data-stu-id="90c57-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="90c57-148">在以下页面上，需要包含星号的字段。</span><span class="sxs-lookup"><span data-stu-id="90c57-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="90c57-149">如果不知道字段的定义，请选择 "信息" 图标。</span><span class="sxs-lookup"><span data-stu-id="90c57-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="90c57-150">在 "**详细信息**" 页上，填写以下字段：**配置文件名称：** 输入唯一名称以标识此付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="90c57-151">**银行帐户位置：** 公司银行所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="90c57-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="90c57-152">**付款方式：** 首选付款方式适用于合作伙伴中心是电子银行传输。</span><span class="sxs-lookup"><span data-stu-id="90c57-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="90c57-153">选择“下一步”。</span><span class="sxs-lookup"><span data-stu-id="90c57-153">Select **Next**.</span></span>

3. <span data-ttu-id="90c57-154">在 "**银行帐户**" 页上，输入你的信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="90c57-155">此页上显示的字段将因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="90c57-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="90c57-156">选择“下一步”。</span><span class="sxs-lookup"><span data-stu-id="90c57-156">Select **Next**.</span></span>

5. <span data-ttu-id="90c57-157">在 "**受益人**" 页上，输入适当的信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="90c57-158">受益人是公司中的人员如果需要讨论你的帐户，则会联系到银行。</span><span class="sxs-lookup"><span data-stu-id="90c57-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="90c57-159">完成这些字段后，选择 "**完成**"，然后选择 "**确认**" 创建银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="90c57-160">你将被重定向到 "**支出和税务配置文件**" 页。</span><span class="sxs-lookup"><span data-stu-id="90c57-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="90c57-161">新配置文件的状态将反映**挂起的 Microsoft 验证**，直到验证完成。</span><span class="sxs-lookup"><span data-stu-id="90c57-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="90c57-162">这可能需要48小时。</span><span class="sxs-lookup"><span data-stu-id="90c57-162">This may take up to 48 hours.</span></span> <span data-ttu-id="90c57-163">验证完成后，你的个人资料状态将反映**已批准**或**需要**执行的操作。</span><span class="sxs-lookup"><span data-stu-id="90c57-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="90c57-164">如果**需要操作**，请重复上述步骤，提供必需的信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="90c57-165">创建税务配置文件</span><span class="sxs-lookup"><span data-stu-id="90c57-165">Create your tax profile</span></span>

<span data-ttu-id="90c57-166">使用以下过程向 Microsoft 提供组织所需的税务信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="90c57-167">本部分中的页面是动态的，将根据你所在的国家或地区而有所不同。</span><span class="sxs-lookup"><span data-stu-id="90c57-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="90c57-168">如果你需要帮助来确定正确的税务信息，请联系你所在国家/地区的相应政府来源。</span><span class="sxs-lookup"><span data-stu-id="90c57-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="90c57-169">对于美洲地区的合作伙伴公司，如果需要有关完成 W8 或 W9 窗体的信息，以下地址会转到 IRS 网站：</span><span class="sxs-lookup"><span data-stu-id="90c57-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="90c57-170">只为公司输入详细信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-170">Enter only details for your company.</span></span> <span data-ttu-id="90c57-171">切勿输入个人详细信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-171">Never enter personal details.</span></span>

1. <span data-ttu-id="90c57-172">在 "**业务配置文件**" 页上，填写必填字段，然后选择 "**下一步**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="90c57-173">在 "**安装**" 页上，选择适用于你的公司的选项。</span><span class="sxs-lookup"><span data-stu-id="90c57-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="90c57-174">如果你的公司仅合并到美国中，或者如果此配置文件适用于个人，请选择左侧的选项。</span><span class="sxs-lookup"><span data-stu-id="90c57-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="90c57-175">如果你的公司在美国外合并，则选择右侧的选项，然后从列表中选择你所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="90c57-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="90c57-176">选择“下一步”。</span><span class="sxs-lookup"><span data-stu-id="90c57-176">Select **Next**.</span></span> 

4. <span data-ttu-id="90c57-177">在 "**税状态**" 页上，输入所需信息，然后选择 "**下一步**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="90c57-178">此页上的字段将因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="90c57-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="90c57-179">详细信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-179">your details.</span></span> 

5. <span data-ttu-id="90c57-180">在 "**其他文档**" 页上，选择 "**下一步**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="90c57-181">选择 "**浏览**" 以上载你所在国家或地区所需的任何文档。</span><span class="sxs-lookup"><span data-stu-id="90c57-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="90c57-182">显示文档名称后，选择 "**上传**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="90c57-183">如果需要删除文档，请选择 "**删除**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="90c57-184">若要保存并继续，请选择 "**完成**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="90c57-185">选择弹出消息中的 "**确认**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="90c57-186">你将返回到 "**支出和税务设置**" 页。</span><span class="sxs-lookup"><span data-stu-id="90c57-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="90c57-187">支出和税务模板常见问题解答</span><span class="sxs-lookup"><span data-stu-id="90c57-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="90c57-188">为什么需要提供费用和/或税务详细信息？</span><span class="sxs-lookup"><span data-stu-id="90c57-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="90c57-189">若要接收 Microsoft 激励计划的付款，需要通过提供有效的支出和税务详细信息来完成注册。</span><span class="sxs-lookup"><span data-stu-id="90c57-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="90c57-190">仅当你提供的支出和税务配置文件由 Microsoft 进行验证时，才会将注册视为已完成。</span><span class="sxs-lookup"><span data-stu-id="90c57-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="90c57-191">如何实现知道我需要提供/更新付出的比率和/或税务详细信息吗？</span><span class="sxs-lookup"><span data-stu-id="90c57-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="90c57-192">在新激励计划中注册的所有合作伙伴都必须提供有效的支出和税务详细信息以完成注册。</span><span class="sxs-lookup"><span data-stu-id="90c57-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="90c57-193">如果激励计划的规则发生更改，或者配置文件的各个方面过期或过期，则可能还需要提供更新的信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="90c57-194">如果发生这种情况，"概述" 页将显示 "需要执行操作" 的状态 **–更新银行和/或税务配置文件**。</span><span class="sxs-lookup"><span data-stu-id="90c57-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="90c57-195">如何提供/更新付款和/或税务详细信息？</span><span class="sxs-lookup"><span data-stu-id="90c57-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="90c57-196">有关如何在合作伙伴中心更新付款和税务详细信息的详细信息，请参阅[如何在合作伙伴中心创建和管理银行和税务配置文件](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span><span class="sxs-lookup"><span data-stu-id="90c57-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="90c57-197">为什么在分配付款和税务配置文件时看不到注册？</span><span class="sxs-lookup"><span data-stu-id="90c57-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="90c57-198">只有 MPN 位置的激励管理员才能创建或管理付款和税务配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="90c57-199">这可能是因为你没有适当的权限，或者你是使用不具有这些权限的帐户登录的。</span><span class="sxs-lookup"><span data-stu-id="90c57-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="90c57-200">请与你的组织管理员联系，以管理银行和税务的权限。</span><span class="sxs-lookup"><span data-stu-id="90c57-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="90c57-201">在哪里可以看到可以使用的我组织的付款和税务配置文件？</span><span class="sxs-lookup"><span data-stu-id="90c57-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="90c57-202">使用以下过程查看支出和税务配置文件：</span><span class="sxs-lookup"><span data-stu-id="90c57-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="90c57-203">登录合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="90c57-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="90c57-204">选择齿轮图标以打开“设置”菜单。</span><span class="sxs-lookup"><span data-stu-id="90c57-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="90c57-205">选择 "**合作伙伴设置**"。</span><span class="sxs-lookup"><span data-stu-id="90c57-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="90c57-206">在“帐户设置”下，选择“付款和税务”，然后选择“付款和税务配置文件”  。</span><span class="sxs-lookup"><span data-stu-id="90c57-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="90c57-207">你将看到所有现有的付款和税务配置文件以及状态和修改功能。</span><span class="sxs-lookup"><span data-stu-id="90c57-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="90c57-208">我的组织正在参与多项激励计划。</span><span class="sxs-lookup"><span data-stu-id="90c57-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="90c57-209">我是否需要多次提供我的付款和税务配置文件？</span><span class="sxs-lookup"><span data-stu-id="90c57-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="90c57-210">通常是由你来自行决定是否使用付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="90c57-211">付款配置文件是在组织级别创建的，这样一来，可以在组织内的多个 MPN ID 和奖励计划中分配相同的银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="90c57-212">在大多数情况下，可以重复使用现有的配置文件或创建新的配置文件。</span><span class="sxs-lookup"><span data-stu-id="90c57-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="90c57-213">但可能也有例外，例如将银行配置文件应用于不同的国家或地区时，因为当地银行或税务规定可能会适用。</span><span class="sxs-lookup"><span data-stu-id="90c57-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="90c57-214">当某一 MPN 位置参与其他奖励计划时，将重用为该 MPN 位置创建的税务配置文件并且会自动进行填充。</span><span class="sxs-lookup"><span data-stu-id="90c57-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="90c57-215">但是可能存在例外情况。</span><span class="sxs-lookup"><span data-stu-id="90c57-215">But there can be exceptions.</span></span> <span data-ttu-id="90c57-216">例如，新的奖励计划的付款规则可能需要其他的税务配置文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="90c57-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="90c57-217">我只能用我的 @onmicrosoft.com 域登录。</span><span class="sxs-lookup"><span data-stu-id="90c57-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="90c57-218">  应采取何种操作？</span><span class="sxs-lookup"><span data-stu-id="90c57-218">What should I do?</span></span>

<span data-ttu-id="90c57-219">请联系你的帐户管理员，将其他域添加到 AAD 帐户。</span><span class="sxs-lookup"><span data-stu-id="90c57-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
