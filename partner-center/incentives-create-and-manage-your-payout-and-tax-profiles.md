---
title: 合作伙伴中心中的付款和税务配置文件
ms.topic: how-to
ms.date: 04/15/2021
description: 创建并管理你的支出和税务配置文件，以便你可以为奖励工作付费。 包括创建、管理和使用不同的配置文件。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 4a931f1d971ea3e3bc288f70e85a6600596761cc
ms.sourcegitcommit: 9f6be9bc8d9a065422d1ec8388bd770eb6cd9f33
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "107528557"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a2b55-104">在合作伙伴中心创建和管理激励支出和税务配置文件</span><span class="sxs-lookup"><span data-stu-id="a2b55-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a2b55-105">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="a2b55-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a2b55-106">奖励管理员</span><span class="sxs-lookup"><span data-stu-id="a2b55-106">Incentives admin</span></span>
- <span data-ttu-id="a2b55-107">帐户管理员</span><span class="sxs-lookup"><span data-stu-id="a2b55-107">Account admin</span></span>
- <span data-ttu-id="a2b55-108">全局管理员</span><span class="sxs-lookup"><span data-stu-id="a2b55-108">Global admin</span></span>

<span data-ttu-id="a2b55-109">必须首先通过将有效的付款和税务配置文件与奖励计划和 MPN 位置相关联来完成注册，然后才能收到针对特定 MPN 位置的奖励计划的付款。</span><span class="sxs-lookup"><span data-stu-id="a2b55-109">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="a2b55-110">Microsoft 将使用此付款和税务配置文件来发放款项。</span><span class="sxs-lookup"><span data-stu-id="a2b55-110">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="a2b55-111">根据具体的奖励计划规则，你可以使用电子银行转帐或贷方通知单来接收付款。</span><span class="sxs-lookup"><span data-stu-id="a2b55-111">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a><span data-ttu-id="a2b55-112">角色、货币和多个 Microsoft 激励计划</span><span class="sxs-lookup"><span data-stu-id="a2b55-112">Roles, currencies, and multiple Microsoft incentive programs</span></span>

<span data-ttu-id="a2b55-113">在开始进行支出和税务分析之前，请务必了解下面的信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-113">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="a2b55-114">角色和权限</span><span class="sxs-lookup"><span data-stu-id="a2b55-114">Roles and permissions</span></span>

<span data-ttu-id="a2b55-115">您必须是一种激励管理员，才能输入银行和税务信息以进行激励支付。</span><span class="sxs-lookup"><span data-stu-id="a2b55-115">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="a2b55-116">如果你是 MPN/帐户管理员，则可以将自己和/或同事分配为奖励管理员。</span><span class="sxs-lookup"><span data-stu-id="a2b55-116">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="a2b55-117">如果需要请求激励管理员权限，请联系 MPN 管理员或全局管理员。你可以通过登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)来找出你的公司中的谁有这些角色。</span><span class="sxs-lookup"><span data-stu-id="a2b55-117">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="a2b55-118">在右上角的 " **设置** " 图标中，选择 " **用户管理** "，然后在 "全局管理员" 上筛选。</span><span class="sxs-lookup"><span data-stu-id="a2b55-118">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="a2b55-119">奖励，用户可以查看激励收益和支付详细信息和报告，但不能编辑银行和税务详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-119">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="a2b55-120">选择付款币种</span><span class="sxs-lookup"><span data-stu-id="a2b55-120">Choose your disbursement currency</span></span>

<span data-ttu-id="a2b55-121">采用在设置付款配置文件时所选的货币进行激励支付。</span><span class="sxs-lookup"><span data-stu-id="a2b55-121">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="a2b55-122">将使用 Microsoft 每月设置的汇率来计算付款。</span><span class="sxs-lookup"><span data-stu-id="a2b55-122">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="a2b55-123">由于所选的货币，你将负责对值所做的任何更改。</span><span class="sxs-lookup"><span data-stu-id="a2b55-123">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="a2b55-124">为不同的 Microsoft 程序使用不同的配置文件</span><span class="sxs-lookup"><span data-stu-id="a2b55-124">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="a2b55-125">如果你的公司注册了多个激励计划，你可以对所有这些计划使用同一支付帐户，或者为不同的程序选择使用不同的付款帐户。</span><span class="sxs-lookup"><span data-stu-id="a2b55-125">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="a2b55-126">在合作伙伴中心创建和管理付款资料和税务资料</span><span class="sxs-lookup"><span data-stu-id="a2b55-126">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="a2b55-127">以下各节将引导你完成在合作伙伴中心创建和管理付款和税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="a2b55-127">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="a2b55-128">您必须是激励管理员才能在合作伙伴中心创建或管理付款和税务配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-128">You must be an Incentive admin to create or manage payment and tax profiles in Partner Center.</span></span> <span data-ttu-id="a2b55-129">奖励角色必须分配给每个激励计划下的每个 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="a2b55-129">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="a2b55-130">有关如何在合作伙伴中心添加激励管理员的详细信息，请参阅 [创建用户帐户](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="a2b55-130">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="a2b55-131">访问合作伙伴中心的支出和税务部分</span><span class="sxs-lookup"><span data-stu-id="a2b55-131">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="a2b55-132">使用你的 Azure Active Directory (Azure AD) 帐户 (公司帐户) ，或使用适当的电子邮件地址（如果已分配）登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/) 。</span><span class="sxs-lookup"><span data-stu-id="a2b55-132">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="a2b55-133">可以在一个 Azure AD 帐户中注册多个域。</span><span class="sxs-lookup"><span data-stu-id="a2b55-133">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="a2b55-134">请与全局管理员联系，以确定与哪些域相关联。</span><span class="sxs-lookup"><span data-stu-id="a2b55-134">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="a2b55-135">如果只能用域登录， @onmicrosoft.com 并且需要其他域，请与帐户管理员联系，将其他域添加到 Azure AD 帐户中。</span><span class="sxs-lookup"><span data-stu-id="a2b55-135">If you're only able to sign in with the @onmicrosoft.com domain and you need additional domains, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="a2b55-136">如果系统提示你选择 **工作或学校帐户** 或 **个人帐户**，请选择 " **工作或学校帐户**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-136">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="a2b55-137">选择齿轮图标以打开 " **设置** " 菜单，然后选择 " **帐户设置**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-137">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="a2b55-138">在 " **帐户设置** " 菜单中，选择 " **支出和税金**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-138">In the **Account settings** menu, select **Payout and tax**.</span></span>

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="a2b55-139">将支出和税务配置文件分配给单个计划</span><span class="sxs-lookup"><span data-stu-id="a2b55-139">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="a2b55-140">登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)，并选择齿轮图标以打开 " **设置** " 菜单。</span><span class="sxs-lookup"><span data-stu-id="a2b55-140">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="a2b55-141">选择 " **帐户设置**"，展开 " **支出和税务" 部分**，然后选择 " **支出和税务配置文件分配**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-141">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="a2b55-142">将显示你的程序列表。</span><span class="sxs-lookup"><span data-stu-id="a2b55-142">A list of your programs will be displayed.</span></span> <span data-ttu-id="a2b55-143">选择程序旁边的箭头以查看配置文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-143">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="a2b55-144">在 " **税务配置文件** " 下拉菜单中，选择所需的税务配置文件，或选择 "创建新配置文件" 选项。</span><span class="sxs-lookup"><span data-stu-id="a2b55-144">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a2b55-145">选择用于创建新配置文件的选项时，会相应地重定向。</span><span class="sxs-lookup"><span data-stu-id="a2b55-145">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="a2b55-146">在弹出窗口中选择 " **继续** "。</span><span class="sxs-lookup"><span data-stu-id="a2b55-146">Select **Continue** in the pop-up window.</span></span> <span data-ttu-id="a2b55-147">下面提供了创建新的税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="a2b55-147">The process for creating a new tax profile is provided below.</span></span>

4. <span data-ttu-id="a2b55-148">选择 " **付款方式**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-148">Select **Payment method**.</span></span>

   - <span data-ttu-id="a2b55-149">如果已选择 " **电子银行传输** " 作为付款方式，请选择所需的付款配置文件，或选择 "创建新配置文件" 选项。</span><span class="sxs-lookup"><span data-stu-id="a2b55-149">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="a2b55-150">选择用于创建新配置文件的选项时，会相应地重定向。</span><span class="sxs-lookup"><span data-stu-id="a2b55-150">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="a2b55-151">在弹出窗口中选择 "继续"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-151">Select Continue in the pop-up window.</span></span> <span data-ttu-id="a2b55-152">下面提供了创建新付款配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="a2b55-152">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="a2b55-153">如果已选择 " **贷方注释** " 作为付款方式，请完成验证。</span><span class="sxs-lookup"><span data-stu-id="a2b55-153">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="a2b55-154">这会确认引用的 SAP 编号属于你的组织。</span><span class="sxs-lookup"><span data-stu-id="a2b55-154">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a2b55-155">如果列出了多个 Microsoft 业务实体，则必须为每个实体选择付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-155">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="a2b55-156">付款方式的可用性取决于激励计划的规则。</span><span class="sxs-lookup"><span data-stu-id="a2b55-156">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="a2b55-157">如果你的位置 MPN ID 由本地 Microsoft 子公司支付给特定激励计划，并允许 LRD (有限的风险分销商) 贷项通知单作为付款方式，则将使用 LRD 信用说明支付方法预填充你的付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-157">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="a2b55-158">在相应激励计划和位置 MPN ID 的 "LRD 贷方通知单支付方法" 行上，你将看到 "需要 **确认** " 或 " **验证** " 作为 "付款配置文件" 部分中的状态。</span><span class="sxs-lookup"><span data-stu-id="a2b55-158">On the LRD credit note payment method row for the respective incentive program and location MPN ID you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="a2b55-159">选择 " **需要验证** "，确认并验证与 "位置 MPN" 和 "付款方式" 相关联的 CSP 租户 ID 详细信息，以接收贷方便笺支付。</span><span class="sxs-lookup"><span data-stu-id="a2b55-159">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="a2b55-160">在 " **贷方注释详细信息** " 对话框中，查看并验证提供的 CSP 租户 ID 和详细信息是否正确。</span><span class="sxs-lookup"><span data-stu-id="a2b55-160">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="a2b55-161">如果显示了多个租户 ID，请仔细选择要接收付款的 CSP 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="a2b55-161">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="a2b55-162">接下来，选择 " **确认** " 以确认你的公司详细信息正确，并且应将激励付款应用于所选的 CSP 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="a2b55-162">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="a2b55-163">如果状态显示为 "已 **确认**"，则 CSP 租户 ID 的分配已完成，无需执行其他操作。</span><span class="sxs-lookup"><span data-stu-id="a2b55-163">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="a2b55-164">你仍可以选择 "已确认" 来查看分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-164">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="a2b55-165">如果国家/地区要求合作伙伴显式请求应用免税，则在激励计划和位置 MPN 的税务分析部分中，将会有一个用于应用税务申报旁边的免税的选项。</span><span class="sxs-lookup"><span data-stu-id="a2b55-165">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="a2b55-166">如果选中此框，则会将免税权益应用到激励贷方注释。</span><span class="sxs-lookup"><span data-stu-id="a2b55-166">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="a2b55-167">目前，LRD 贷方通知单支付方法仅适用于 Microsoft 商业激励计划的澳大利亚、新西兰和加拿大合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="a2b55-167">Currently, the LRD Credit Note payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="a2b55-168">如果你是注册了 MCI 计划的这三个国家/地区的直接帐单合作伙伴或间接提供商，但没有看到 LRD 贷方注释作为可用的付款方式，请确认你的租户 ID 与相关的合作伙伴 MPN 位置帐户关联。</span><span class="sxs-lookup"><span data-stu-id="a2b55-168">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="a2b55-169">有关此内容的详细信息，请参阅 [如何更新组织配置文件](update-your-partner-profile.md)。</span><span class="sxs-lookup"><span data-stu-id="a2b55-169">For more information on this read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="a2b55-170">选择 **货币**。</span><span class="sxs-lookup"><span data-stu-id="a2b55-170">Select the **Currency**.</span></span>

6. <span data-ttu-id="a2b55-171">完成所有付款字段后，选择 " **提交**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-171">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="set-up-a-default-bank-profile"></a><span data-ttu-id="a2b55-172">设置默认银行配置文件</span><span class="sxs-lookup"><span data-stu-id="a2b55-172">Set up a default bank profile</span></span>

<span data-ttu-id="a2b55-173">可以设置默认的银行配置文件并将其分配到 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="a2b55-173">You can setup default bank profiles and assign them to MPN locations.</span></span> <span data-ttu-id="a2b55-174">Microsoft 将使用这些默认配置文件，以便以后注册该 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="a2b55-174">These defaults profiles will be used by Microsoft for subsequent enrollments for that MPN location.</span></span> 

1. <span data-ttu-id="a2b55-175">登录到[合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)，并选择齿轮图标以打开 "设置" \*\*\*\*   菜单。</span><span class="sxs-lookup"><span data-stu-id="a2b55-175">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/),  and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="a2b55-176">选择 " **帐户设置**"，展开 " **支出和税务** " 部分，然后选择 " **支出和税务配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-176">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profiles**.</span></span> 

3. <span data-ttu-id="a2b55-177">选择 "**付款配置文件**" 部分下的 "**管理默认配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-177">Select **Manage default profiles** under the **Payment profiles** section.</span></span> 

4. <span data-ttu-id="a2b55-178">若要创建默认银行配置文件，请选择 " **添加默认银行配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-178">To create a default bank profiles select **Add a default bank profile**.</span></span> 

5. <span data-ttu-id="a2b55-179">从公司的可用银行配置文件列表中选择银行配置文件，选择要与此银行配置文件一起使用的货币，然后选择要应用此默认配置文件的 MPN 位置的列表。</span><span class="sxs-lookup"><span data-stu-id="a2b55-179">Select a bank profile from the list of available bank profiles of your company, select the currency to be used with this bank profile, and then select the list of MPN locations for which you want this default profile to apply.</span></span>

6. <span data-ttu-id="a2b55-180">完成选择后，选择 " **完成** "。</span><span class="sxs-lookup"><span data-stu-id="a2b55-180">Select **Done** once you have completed the selections.</span></span> <span data-ttu-id="a2b55-181">完成所需的所有字段后，"完成" 按钮才会单击。</span><span class="sxs-lookup"><span data-stu-id="a2b55-181">The Done button will not be clickable until all required fields have been completed.</span></span> 

>[!NOTE]
><span data-ttu-id="a2b55-182">同一银行和币种配对可以应用于多个位置。</span><span class="sxs-lookup"><span data-stu-id="a2b55-182">The same bank and currency pairing can be applied to multiple locations.</span></span> <span data-ttu-id="a2b55-183">如果已将默认配置文件和货币组合分配给位置 MPN，则它将不再出现在将来的默认配置文件分配的 "位置" 下拉列表中。</span><span class="sxs-lookup"><span data-stu-id="a2b55-183">If the location MPN has been assigned a default profile and currency combination once, it will no longer appear in the location dropdown for future default profile assignments.</span></span> <span data-ttu-id="a2b55-184">如果删除了默认选择，则 MPN 将重新出现位置，以供将来的默认配置文件分配。</span><span class="sxs-lookup"><span data-stu-id="a2b55-184">If the default selection is deleted, the location MPN will reappear for future default profile assignments.</span></span> <span data-ttu-id="a2b55-185">每个银行配置文件和货币组合将添加为唯一的可编辑行。</span><span class="sxs-lookup"><span data-stu-id="a2b55-185">Each bank profile and currency combination is added as an unique, editable row.</span></span>

7. <span data-ttu-id="a2b55-186">添加所有必需的更改后，请选择 " **保存**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-186">Once all the required changes have been added, select **Save**.</span></span>  

## <a name="create-your-bank-profile"></a><span data-ttu-id="a2b55-187">创建银行配置文件</span><span class="sxs-lookup"><span data-stu-id="a2b55-187">Create your bank profile</span></span>

<span data-ttu-id="a2b55-188">银行配置文件在公司级别创建。</span><span class="sxs-lookup"><span data-stu-id="a2b55-188">Bank profiles are created at an company level.</span></span> <span data-ttu-id="a2b55-189">这允许在一个公司内跨多个 MPN ID 和激励计划分配一个银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-189">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within a company.</span></span> <span data-ttu-id="a2b55-190">将银行配置文件应用于不同的国家/地区时，可能会出现例外，因为不同的银行和税务规则可能适用。</span><span class="sxs-lookup"><span data-stu-id="a2b55-190">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="a2b55-191">在以下页面上，需要包含星号的字段。</span><span class="sxs-lookup"><span data-stu-id="a2b55-191">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="a2b55-192">如果不知道字段的定义，请选择 "信息" 图标。</span><span class="sxs-lookup"><span data-stu-id="a2b55-192">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="a2b55-193">在 " **详细信息** " 页上，填写以下字段： **配置文件名称：** 输入唯一名称以标识此付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-193">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="a2b55-194">**银行帐户位置：** 公司银行所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="a2b55-194">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="a2b55-195">**付款方式：** 合作伙伴中心的首选付款方式是电子银行传输。</span><span class="sxs-lookup"><span data-stu-id="a2b55-195">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="a2b55-196">选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="a2b55-196">Select **Next**.</span></span>

3. <span data-ttu-id="a2b55-197">在 " **银行帐户** " 页上，输入你的信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-197">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="a2b55-198">此页上显示的字段将因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="a2b55-198">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="a2b55-199">选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="a2b55-199">Select **Next**.</span></span>

5. <span data-ttu-id="a2b55-200">在 " **受益人** " 页上，输入适当的信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-200">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="a2b55-201">受益人是公司中的人员如果需要讨论你的帐户，则会联系到银行。</span><span class="sxs-lookup"><span data-stu-id="a2b55-201">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="a2b55-202">完成这些字段后，选择 " **完成**"，然后选择 " **确认** " 创建银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-202">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="a2b55-203">你将被重定向到 " **支出和税务配置文件** " 页。</span><span class="sxs-lookup"><span data-stu-id="a2b55-203">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="a2b55-204">新配置文件的状态将反映 **挂起的 Microsoft 验证** ，直到验证完成。</span><span class="sxs-lookup"><span data-stu-id="a2b55-204">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="a2b55-205">此过程最多可能需要48小时。</span><span class="sxs-lookup"><span data-stu-id="a2b55-205">This process may take up to 48 hours.</span></span> <span data-ttu-id="a2b55-206">验证完成后，你的个人资料状态将反映 **已批准** 或 **需要** 执行的操作。</span><span class="sxs-lookup"><span data-stu-id="a2b55-206">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="a2b55-207">如果 **需要操作**，请重复上述步骤，提供必需的信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-207">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="a2b55-208">创建税务配置文件</span><span class="sxs-lookup"><span data-stu-id="a2b55-208">Create your tax profile</span></span>

<span data-ttu-id="a2b55-209">使用以下过程向 Microsoft 提供组织所需的税务信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-209">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="a2b55-210">本部分中的页面是动态的，将根据你所在的国家或地区而有所不同。</span><span class="sxs-lookup"><span data-stu-id="a2b55-210">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="a2b55-211">如果你需要帮助来确定正确的税务信息，请联系你所在国家/地区的相应政府来源。</span><span class="sxs-lookup"><span data-stu-id="a2b55-211">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="a2b55-212">对于美洲地区的合作伙伴公司，如果需要有关完成 W8 或 W9 窗体的信息，以下地址会转到 IRS 网站：</span><span class="sxs-lookup"><span data-stu-id="a2b55-212">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="a2b55-213">只为公司输入详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-213">Enter only details for your company.</span></span> <span data-ttu-id="a2b55-214">切勿输入个人详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-214">Never enter personal details.</span></span>

1. <span data-ttu-id="a2b55-215">在 " **业务配置文件** " 页上，填写必填字段，然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-215">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="a2b55-216">在 " **安装** " 页上，选择适用于你的公司的选项。</span><span class="sxs-lookup"><span data-stu-id="a2b55-216">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="a2b55-217">如果你的公司仅合并到美国中，或者如果此配置文件适用于个人，请选择左侧的选项。</span><span class="sxs-lookup"><span data-stu-id="a2b55-217">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="a2b55-218">如果你的公司在美国外合并，则选择右侧的选项，然后从列表中选择你所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="a2b55-218">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="a2b55-219">选择“下一步”  。</span><span class="sxs-lookup"><span data-stu-id="a2b55-219">Select **Next**.</span></span> 

4. <span data-ttu-id="a2b55-220">在 " **税状态** " 页上，输入所需信息，然后选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-220">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="a2b55-221">此页上的字段将因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="a2b55-221">Fields on this page will vary by country.</span></span> <span data-ttu-id="a2b55-222">详细信息。</span><span class="sxs-lookup"><span data-stu-id="a2b55-222">your details.</span></span> 

5. <span data-ttu-id="a2b55-223">在 " **其他文档** " 页上，选择 " **下一步**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-223">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="a2b55-224">选择 " **浏览** " 以上载你所在国家或地区所需的任何文档。</span><span class="sxs-lookup"><span data-stu-id="a2b55-224">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="a2b55-225">显示文档名称后，选择 " **上传**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-225">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="a2b55-226">如果需要删除文档，请选择 " **删除**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-226">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="a2b55-227">若要保存并继续，请选择 " **完成**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-227">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="a2b55-228">选择弹出消息中的 " **确认** "。</span><span class="sxs-lookup"><span data-stu-id="a2b55-228">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="a2b55-229">你将返回到 " **支出和税务设置** " 页。</span><span class="sxs-lookup"><span data-stu-id="a2b55-229">You’ll be taken back to the **Payout and tax setup** page.</span></span>
 
## <a name="update-expired-tax-profiles"></a><span data-ttu-id="a2b55-230">更新过期的税务配置文件</span><span class="sxs-lookup"><span data-stu-id="a2b55-230">Update expired tax profiles</span></span>

1. <span data-ttu-id="a2b55-231">登录到 [合作伙伴中心仪表板](https://partner.microsoft.com/dashboard/)，并选择齿轮图标以打开 " **设置** " 菜单。</span><span class="sxs-lookup"><span data-stu-id="a2b55-231">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span>

1. <span data-ttu-id="a2b55-232">选择 " **帐户设置**"，展开 " **支出和税务** " 部分，然后选择 " **支出和税务配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-232">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profile**.</span></span>

1. <span data-ttu-id="a2b55-233">选择 " **税务配置文件**"。</span><span class="sxs-lookup"><span data-stu-id="a2b55-233">Select **Tax profile**.</span></span>

1. <span data-ttu-id="a2b55-234">检查列 **到期日期** 并导航到过期的或即将过期的税务配置文件。</span><span class="sxs-lookup"><span data-stu-id="a2b55-234">Check the column **Expiration Date** and navigate to the tax profile that is expired or about to expire.</span></span>

1. <span data-ttu-id="a2b55-235">选择“编辑”。</span><span class="sxs-lookup"><span data-stu-id="a2b55-235">Select **Edit**.</span></span>

1. <span data-ttu-id="a2b55-236">在 "税务窗体" 部分中，通过提供新的详细信息来更新纳税形式。</span><span class="sxs-lookup"><span data-stu-id="a2b55-236">In the tax form section, update the tax forms by providing the new details.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="a2b55-237">后续步骤</span><span class="sxs-lookup"><span data-stu-id="a2b55-237">Next steps</span></span>

- [<span data-ttu-id="a2b55-238">有关付款和税款的常见问题</span><span class="sxs-lookup"><span data-stu-id="a2b55-238">Common questions about payouts and taxes</span></span>](payout-faq.md)
