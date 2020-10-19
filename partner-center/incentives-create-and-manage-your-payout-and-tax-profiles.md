---
title: 合作伙伴中心中的付款和税务配置文件
ms.topic: how-to
ms.date: 09/11/2020
description: 创建并管理你的支出和税务配置文件，以便你可以为奖励工作付费。 包括创建、管理和使用不同的配置文件。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: ca2ffe992ff92b98546934f4a249779f39179acb
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175357"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="fbfc9-104">在合作伙伴中心创建和管理激励支出和税务配置文件</span><span class="sxs-lookup"><span data-stu-id="fbfc9-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="fbfc9-105">**适用对象：**</span><span class="sxs-lookup"><span data-stu-id="fbfc9-105">**Applies to:**</span></span>

- <span data-ttu-id="fbfc9-106">合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="fbfc9-106">Partner Center</span></span>

<span data-ttu-id="fbfc9-107">**相应的角色：**</span><span class="sxs-lookup"><span data-stu-id="fbfc9-107">**Appropriate roles:**</span></span>

- <span data-ttu-id="fbfc9-108">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="fbfc9-108">Incentives admin</span></span>
- <span data-ttu-id="fbfc9-109">计费管理员</span><span class="sxs-lookup"><span data-stu-id="fbfc9-109">Billing admin</span></span>
- <span data-ttu-id="fbfc9-110">全局管理员</span><span class="sxs-lookup"><span data-stu-id="fbfc9-110">Global admin</span></span>

<span data-ttu-id="fbfc9-111">必须首先通过将有效的付款和税务配置文件与奖励计划和 MPN 位置相关联来完成注册，然后才能收到针对特定 MPN 位置的奖励计划的付款。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-111">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="fbfc9-112">Microsoft 将使用此付款和税务配置文件来发放款项。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-112">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="fbfc9-113">根据具体的奖励计划规则，你可以使用电子银行转帐或贷方通知单来接收付款。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-113">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="fbfc9-114">角色、货币和其他 Microsoft 程序</span><span class="sxs-lookup"><span data-stu-id="fbfc9-114">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="fbfc9-115">在开始进行支出和税务分析之前，请务必了解下面的信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-115">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="fbfc9-116">角色和权限</span><span class="sxs-lookup"><span data-stu-id="fbfc9-116">Roles and permissions</span></span>

<span data-ttu-id="fbfc9-117">您必须是一种激励管理员，才能输入银行和税务信息以进行激励支付。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-117">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="fbfc9-118">如果你是 MPN/帐户管理员，则可以将自己和/或同事分配为奖励管理员。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-118">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="fbfc9-119">如果需要请求激励管理员权限，请联系 MPN 管理员或全局管理员。你可以通过登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)来找出你的公司中的谁有这些角色。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-119">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="fbfc9-120">在右上角的 " **设置** " 图标中，选择 " **用户管理** "，然后在 "全局管理员" 上筛选。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-120">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="fbfc9-121">奖励，用户可以查看激励收益和支付详细信息和报告，但不能编辑银行和税务详细信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-121">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="fbfc9-122">选择付款币种</span><span class="sxs-lookup"><span data-stu-id="fbfc9-122">Choose your disbursement currency</span></span>

<span data-ttu-id="fbfc9-123">默认情况下，激励支付以各自实体的本地货币进行。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-123">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="fbfc9-124">可以在配置文件安装过程中指定不同的货币。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-124">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="fbfc9-125">将使用 Microsoft 每月设置的汇率来计算付款。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-125">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="fbfc9-126">由于所选的货币，你将负责对值所做的任何更改。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-126">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="fbfc9-127">银行和税务信息以及其他程序</span><span class="sxs-lookup"><span data-stu-id="fbfc9-127">Bank and tax information and other programs</span></span>

<span data-ttu-id="fbfc9-128">提供下面所述的信息，即使 Microsoft 已使用银行数据支付费用。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-128">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="fbfc9-129">这有助于确保公司数据的隐私性和安全性，因为将您的配置文件复制到新工具可能会暴露敏感信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-129">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="fbfc9-130">完成此过程也是确保数据完整且准确的好机会。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-130">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="fbfc9-131">为不同的 Microsoft 程序使用不同的配置文件</span><span class="sxs-lookup"><span data-stu-id="fbfc9-131">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="fbfc9-132">在零售范围内，这五个零售激励计划中的每一项都可以发送到相同的银行帐户。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-132">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="fbfc9-133">另外，还可以选择在零售办公室支付给不同银行帐户时，将零售 Xbox 付款传入一个银行帐户。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-133">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="fbfc9-134">在合作伙伴中心创建和管理付款资料和税务资料</span><span class="sxs-lookup"><span data-stu-id="fbfc9-134">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="fbfc9-135">以下各节将引导你完成在合作伙伴中心创建和管理付款和税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-135">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="fbfc9-136">您必须是激励管理员才能在合作伙伴中心创建或管理付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-136">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="fbfc9-137">奖励角色必须分配给每个激励计划下的每个 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-137">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="fbfc9-138">有关如何在合作伙伴中心添加激励管理员的详细信息，请参阅 [创建用户帐户](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-138">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="fbfc9-139">访问合作伙伴中心的支出和税务部分</span><span class="sxs-lookup"><span data-stu-id="fbfc9-139">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="fbfc9-140">使用你的 Azure Active Directory (Azure AD) 帐户 (公司帐户) ，或使用适当的电子邮件地址（如果已分配）登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/) 。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="fbfc9-141">可以在一个 Azure AD 帐户中注册多个域。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-141">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="fbfc9-142">请与全局管理员联系，以确定与哪些域相关联。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-142">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="fbfc9-143">如果只能用 @onmicrosoft.com 域登录，请与帐户管理员联系，将其他域添加到 Azure AD 帐户中。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-143">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="fbfc9-144">如果系统提示你选择 **工作或学校帐户** 或 **个人帐户**，请选择 " **工作或学校帐户**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-144">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="fbfc9-145">选择齿轮图标以打开 " **设置** " 菜单，然后选择 " **合作伙伴设置**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-145">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="fbfc9-146">在 " **帐户设置** " 菜单中，选择 " **支出和税金**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-146">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="fbfc9-147">将支出和税务配置文件分配给单个计划</span><span class="sxs-lookup"><span data-stu-id="fbfc9-147">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="fbfc9-148">登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)，并选择齿轮图标以打开 " **设置** " 菜单。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-148">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="fbfc9-149">选择 " **合作伙伴设置**"，展开 " **支出和税务" 部分**，然后选择 " **分配**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-149">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="fbfc9-150">将显示你的程序列表。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-150">A list of your programs will be displayed.</span></span> <span data-ttu-id="fbfc9-151">选择程序旁边的箭头以查看配置文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-151">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="fbfc9-152">在 " **税务配置文件** " 下拉菜单中，选择所需的税务配置文件，或选择 "创建新配置文件" 选项。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-152">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="fbfc9-153">选择用于创建新配置文件的选项时，会相应地重定向。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-153">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="fbfc9-154">在弹出窗口中选择 "继续"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-154">Select Continue in the pop-up window.</span></span> <span data-ttu-id="fbfc9-155">下面提供了创建新的税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-155">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="fbfc9-156">选择 " **付款方式**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-156">Select **Payment method**.</span></span>

   - <span data-ttu-id="fbfc9-157">如果已选择 " **电子银行传输** " 作为付款方式，请选择所需的付款配置文件，或选择 "创建新配置文件" 选项。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-157">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="fbfc9-158">选择用于创建新配置文件的选项时，会相应地重定向。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-158">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="fbfc9-159">在弹出窗口中选择 "继续"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-159">Select Continue in the pop-up window.</span></span> <span data-ttu-id="fbfc9-160">下面提供了创建新付款配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-160">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="fbfc9-161">如果已选择 " **贷方注释** " 作为付款方式，请完成验证。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-161">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="fbfc9-162">这会确认引用的 SAP 编号属于你的组织。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-162">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="fbfc9-163">如果列出了多个 Microsoft 业务实体，则必须为每个实体选择付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-163">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="fbfc9-164">付款方式的可用性取决于激励计划的规则。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-164">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="fbfc9-165">选择 **货币**。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-165">Select the **Currency**.</span></span>

6. <span data-ttu-id="fbfc9-166">完成所有付款字段后，选择 " **提交**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-166">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="fbfc9-167">创建银行配置文件</span><span class="sxs-lookup"><span data-stu-id="fbfc9-167">Create your bank profile</span></span>

<span data-ttu-id="fbfc9-168">银行配置文件在组织级别创建。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-168">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="fbfc9-169">这样，便可以在组织中的多个 MPN ID 和激励程序之间分配一个银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-169">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="fbfc9-170">将银行配置文件应用于不同的国家/地区时，可能会出现例外，因为不同的银行和税务规则可能适用。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-170">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="fbfc9-171">在以下页面上，需要包含星号的字段。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-171">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="fbfc9-172">如果不知道字段的定义，请选择 "信息" 图标。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-172">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="fbfc9-173">在 " **详细信息** " 页上，填写以下字段： **配置文件名称：** 输入唯一名称以标识此付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-173">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="fbfc9-174">**银行帐户位置：** 公司银行所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-174">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="fbfc9-175">**付款方式：** 合作伙伴中心的首选付款方式是电子银行传输。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-175">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="fbfc9-176">选择“**下一页**”。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-176">Select **Next**.</span></span>

3. <span data-ttu-id="fbfc9-177">在 " **银行帐户** " 页上，输入你的信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-177">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="fbfc9-178">此页上显示的字段将因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-178">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="fbfc9-179">选择“**下一页**”。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-179">Select **Next**.</span></span>

5. <span data-ttu-id="fbfc9-180">在 " **受益人** " 页上，输入适当的信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-180">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="fbfc9-181">受益人是公司中的人员如果需要讨论你的帐户，则会联系到银行。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-181">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="fbfc9-182">完成这些字段后，选择 " **完成**"，然后选择 " **确认** " 创建银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-182">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="fbfc9-183">你将被重定向到 " **支出和税务配置文件** " 页。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-183">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="fbfc9-184">新配置文件的状态将反映 **挂起的 Microsoft 验证** ，直到验证完成。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-184">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="fbfc9-185">此过程最多可能需要48小时。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-185">This process may take up to 48 hours.</span></span> <span data-ttu-id="fbfc9-186">验证完成后，你的个人资料状态将反映 **已批准** 或 **需要**执行的操作。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-186">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="fbfc9-187">如果 **需要操作**，请重复上述步骤，提供必需的信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-187">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="fbfc9-188">创建税务配置文件</span><span class="sxs-lookup"><span data-stu-id="fbfc9-188">Create your tax profile</span></span>

<span data-ttu-id="fbfc9-189">使用以下过程向 Microsoft 提供组织所需的税务信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-189">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="fbfc9-190">本部分中的页面是动态的，将根据你所在的国家或地区而有所不同。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-190">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="fbfc9-191">如果你需要帮助来确定正确的税务信息，请联系你所在国家/地区的相应政府来源。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-191">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="fbfc9-192">对于美洲地区的合作伙伴公司，如果需要有关完成 W8 或 W9 窗体的信息，以下地址会转到 IRS 网站：</span><span class="sxs-lookup"><span data-stu-id="fbfc9-192">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="fbfc9-193">只为公司输入详细信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-193">Enter only details for your company.</span></span> <span data-ttu-id="fbfc9-194">切勿输入个人详细信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-194">Never enter personal details.</span></span>

1. <span data-ttu-id="fbfc9-195">在 " **业务配置文件** " 页上，填写必填字段，然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-195">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="fbfc9-196">在 " **安装** " 页上，选择适用于你的公司的选项。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-196">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="fbfc9-197">如果你的公司仅合并到美国中，或者如果此配置文件适用于个人，请选择左侧的选项。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-197">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="fbfc9-198">如果你的公司在美国外合并，则选择右侧的选项，然后从列表中选择你所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-198">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="fbfc9-199">选择“**下一页**”。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-199">Select **Next**.</span></span> 

4. <span data-ttu-id="fbfc9-200">在 " **税状态** " 页上，输入所需信息，然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-200">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="fbfc9-201">此页上的字段将因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-201">Fields on this page will vary by country.</span></span> <span data-ttu-id="fbfc9-202">详细信息。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-202">your details.</span></span> 

5. <span data-ttu-id="fbfc9-203">在 " **其他文档** " 页上，选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-203">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="fbfc9-204">选择 " **浏览** " 以上载你所在国家或地区所需的任何文档。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-204">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="fbfc9-205">显示文档名称后，选择 " **上传**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-205">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="fbfc9-206">如果需要删除文档，请选择 " **删除**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-206">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="fbfc9-207">若要保存并继续，请选择 " **完成**"。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-207">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="fbfc9-208">选择弹出消息中的 " **确认** "。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-208">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="fbfc9-209">你将返回到 " **支出和税务设置** " 页。</span><span class="sxs-lookup"><span data-stu-id="fbfc9-209">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fbfc9-210">后续步骤</span><span class="sxs-lookup"><span data-stu-id="fbfc9-210">Next steps</span></span>

- [<span data-ttu-id="fbfc9-211">关于奖励付款和税务资料的常见问题解答</span><span class="sxs-lookup"><span data-stu-id="fbfc9-211">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
