---
title: 合作伙伴中心中的付款和税务配置文件
ms.topic: how-to
ms.date: 04/15/2021
description: 创建和管理付款和税务配置文件，以便你获得奖励工作的付款。 包括创建、管理和使用不同的配置文件。
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: a6d578c2ad09e1f8bb03f520d659f1a9b1e199a9
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684247"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="3030d-104">在公司创建和管理奖励付款和税务合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="3030d-104">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="3030d-105">**适当角色**：奖励管理员|帐户管理员|全局管理员</span><span class="sxs-lookup"><span data-stu-id="3030d-105">**Appropriate roles**: Incentives admin | Account admin | Global admin</span></span>

<span data-ttu-id="3030d-106">必须首先通过将有效的付款和税务配置文件与奖励计划和 MPN 位置相关联来完成注册，然后才能收到针对特定 MPN 位置的奖励计划的付款。</span><span class="sxs-lookup"><span data-stu-id="3030d-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="3030d-107">Microsoft 将使用此付款和税务配置文件来发放款项。</span><span class="sxs-lookup"><span data-stu-id="3030d-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="3030d-108">根据具体的奖励计划规则，你可以使用电子银行转帐或贷方通知单来接收付款。</span><span class="sxs-lookup"><span data-stu-id="3030d-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-multiple-microsoft-incentive-programs"></a><span data-ttu-id="3030d-109">角色、货币和多个 Microsoft 奖励计划</span><span class="sxs-lookup"><span data-stu-id="3030d-109">Roles, currencies, and multiple Microsoft incentive programs</span></span>

<span data-ttu-id="3030d-110">在开始付款和税务配置文件之前，必须了解以下信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-110">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="3030d-111">角色和权限</span><span class="sxs-lookup"><span data-stu-id="3030d-111">Roles and permissions</span></span>

<span data-ttu-id="3030d-112">你必须是奖励管理员才能输入奖励付款的银行和税务信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-112">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="3030d-113">如果你是 MPN/帐户管理员，可以为自己和/或同事分配为奖励管理员。</span><span class="sxs-lookup"><span data-stu-id="3030d-113">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="3030d-114">如果需要请求奖励管理员权限，请联系 MPN 管理员或全局管理员。可以通过登录仪表板 来查找公司中具有这些角色 [合作伙伴中心角色](https://partner.microsoft.com/dashboard/)。</span><span class="sxs-lookup"><span data-stu-id="3030d-114">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="3030d-115">在右上角 **设置** 图标中，选择"**用户** 管理"，然后筛选"全局管理员"。</span><span class="sxs-lookup"><span data-stu-id="3030d-115">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="3030d-116">奖励 用户可以查看奖励收益和付款详细信息和报表，但不能编辑银行和税务详细信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-116">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="3030d-117">选择货币</span><span class="sxs-lookup"><span data-stu-id="3030d-117">Choose your disbursement currency</span></span>

<span data-ttu-id="3030d-118">奖励付款以设置付款配置文件时选择的货币进行。</span><span class="sxs-lookup"><span data-stu-id="3030d-118">Incentive payments are made in the currency you selected when you set up your payment profile.</span></span> <span data-ttu-id="3030d-119">付款将按 Microsoft 每月设置汇率进行计算。</span><span class="sxs-lookup"><span data-stu-id="3030d-119">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="3030d-120">你将负责因所选货币而对值进行的任何更改。</span><span class="sxs-lookup"><span data-stu-id="3030d-120">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="3030d-121">对不同的 Microsoft 程序使用不同的配置文件</span><span class="sxs-lookup"><span data-stu-id="3030d-121">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="3030d-122">如果你的公司注册了多个奖励计划，你可以对所有这些计划使用相同的付款帐户，或者选择使用不同的付款帐户来实施不同的计划。</span><span class="sxs-lookup"><span data-stu-id="3030d-122">If your company is enrolled in multiple incentive programs, you can use the same payment account for all of them, or choose to use different payment accounts for different programs.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="3030d-123">在合作伙伴中心创建和管理付款资料和税务资料</span><span class="sxs-lookup"><span data-stu-id="3030d-123">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="3030d-124">以下部分将介绍在客户中创建和管理付款和税务配置文件合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="3030d-124">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="3030d-125">你必须是奖励管理员，才能创建或管理付款和税务配置文件合作伙伴中心。</span><span class="sxs-lookup"><span data-stu-id="3030d-125">You must be an Incentive admin to create or manage payment and tax profiles in Partner Center.</span></span> <span data-ttu-id="3030d-126">奖励角色必须分配到每个奖励计划下的每个 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="3030d-126">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="3030d-127">若要详细了解如何在 合作伙伴中心 中添加奖励管理员，请参阅 [创建用户帐户](create-user-accounts-and-set-permissions.md)。</span><span class="sxs-lookup"><span data-stu-id="3030d-127">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="3030d-128">访问"付款和税务"部分合作伙伴中心</span><span class="sxs-lookup"><span data-stu-id="3030d-128">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="3030d-129">使用公司[合作伙伴中心](https://partner.microsoft.com/dashboard/)帐户登录 Azure Active Directory (Azure AD) 仪表板 (公司帐户) 或分配相应的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3030d-129">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="3030d-130">可以在一个帐户内注册Azure AD域。</span><span class="sxs-lookup"><span data-stu-id="3030d-130">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="3030d-131">请与全局管理员联系，确定关联的域。</span><span class="sxs-lookup"><span data-stu-id="3030d-131">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="3030d-132">如果只能使用域登录并且需要其他域，请联系帐户管理员，将其他域添加到Azure AD @onmicrosoft.com 帐户。</span><span class="sxs-lookup"><span data-stu-id="3030d-132">If you're only able to sign in with the @onmicrosoft.com domain and you need additional domains, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="3030d-133">如果系统提示选择"工作或 **学校** 帐户"或"**个人帐户"，请选择**"**工作或学校帐户"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-133">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="3030d-134">选择齿轮图标以打开 **设置菜单，** 然后选择"帐户 **设置"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-134">Select the gear icon to open the **Settings** menu, and then select **Account settings**.</span></span>

3. <span data-ttu-id="3030d-135">在"**帐户设置"菜单中**，选择"**付款和税务"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-135">In the **Account settings** menu, select **Payout and tax**.</span></span>

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="3030d-136">将付款和税务配置文件分配给单个计划</span><span class="sxs-lookup"><span data-stu-id="3030d-136">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="3030d-137">登录到 合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/)，然后选择齿轮图标以 **打开设置菜单**。</span><span class="sxs-lookup"><span data-stu-id="3030d-137">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="3030d-138">选择 **"帐户设置**"，展开"**付款和税务"** 部分，然后选择"**付款和税务配置文件分配"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-138">Select **Account settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="3030d-139">将显示程序列表。</span><span class="sxs-lookup"><span data-stu-id="3030d-139">A list of your programs will be displayed.</span></span> <span data-ttu-id="3030d-140">选择程序旁边的箭头以查看配置文件详细信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-140">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="3030d-141">在" **税务配置文件** "下拉菜单中，选择你需要的税务配置文件，或选择用于创建新配置文件的选项。</span><span class="sxs-lookup"><span data-stu-id="3030d-141">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="3030d-142">选择创建新配置文件的选项时，将正确重定向。</span><span class="sxs-lookup"><span data-stu-id="3030d-142">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="3030d-143">在 **弹出窗口** 中选择"继续"。</span><span class="sxs-lookup"><span data-stu-id="3030d-143">Select **Continue** in the pop-up window.</span></span> <span data-ttu-id="3030d-144">下面提供了创建新税务配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="3030d-144">The process for creating a new tax profile is provided below.</span></span>

4. <span data-ttu-id="3030d-145">选择 **"付款方式"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-145">Select **Payment method**.</span></span>

   - <span data-ttu-id="3030d-146">如果已选择" **电子银行** 转让"作为付款方式，请选择你选择的付款配置文件，或选择用于创建新配置文件的选项。</span><span class="sxs-lookup"><span data-stu-id="3030d-146">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="3030d-147">选择创建新配置文件的选项时，将正确重定向。</span><span class="sxs-lookup"><span data-stu-id="3030d-147">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="3030d-148">在弹出窗口中选择"继续"。</span><span class="sxs-lookup"><span data-stu-id="3030d-148">Select Continue in the pop-up window.</span></span> <span data-ttu-id="3030d-149">下面提供了创建新付款配置文件的过程。</span><span class="sxs-lookup"><span data-stu-id="3030d-149">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="3030d-150">如果已选择" **信用额度** "作为付款方式，请完成验证。</span><span class="sxs-lookup"><span data-stu-id="3030d-150">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="3030d-151">这确认引用的 SAP 编号属于你的组织。</span><span class="sxs-lookup"><span data-stu-id="3030d-151">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3030d-152">如果列出了多个 Microsoft 业务实体，则必须选择每个实体的付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="3030d-152">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="3030d-153">付款方式的可用性取决于奖励计划的规则。</span><span class="sxs-lookup"><span data-stu-id="3030d-153">The payment method availability is dependent on the rules of the incentive program.</span></span>

    - <span data-ttu-id="3030d-154">如果你的位置 MPN ID 由本地 Microsoft 子公司为特定奖励计划付费，并允许 LRD (有限风险分发服务器) 信用额度作为付款方式，则付款配置文件将预先填充 LRD 信用额度付款方式。</span><span class="sxs-lookup"><span data-stu-id="3030d-154">If your location MPN ID is paid by a local Microsoft subsidiary for a particular incentive program and allows LRD (limited risk distributor) credit memo as the payment method, then your payment profile will be pre-populated with the LRD Credit Note payment method.</span></span> <span data-ttu-id="3030d-155">在相应奖励计划以及位置 MPN ID 的 LRD 信用额度付款方式行中，你将在付款配置文件部分看到"已确认"或"需要验证"作为状态。</span><span class="sxs-lookup"><span data-stu-id="3030d-155">On the LRD credit note payment method row for the respective incentive program and location MPN ID, you will see **Confirmed** or **Verification Needed** as the status in the payment profile section.</span></span>
    
       <span data-ttu-id="3030d-156">选择 **"需要** 验证"以确认并验证与位置 MPN 和付款方式关联的 CSP 租户 ID 详细信息，以接收信用额度付款。</span><span class="sxs-lookup"><span data-stu-id="3030d-156">Select **Verification needed** to confirm and verify the CSP tenant ID details that are associated with the location MPN and payment method to receive the credit note payment.</span></span> <span data-ttu-id="3030d-157">在" **信用注释详细信息** "对话框中，查看并验证提供的 CSP 租户 ID 和详细信息是否正确。</span><span class="sxs-lookup"><span data-stu-id="3030d-157">In the **Credit Note Details** dialog box, review and verify that the CSP Tenant ID and details provided are correct.</span></span> <span data-ttu-id="3030d-158">如果看到多个租户 ID，请仔细选择要接收付款的 CSP 租户 ID。</span><span class="sxs-lookup"><span data-stu-id="3030d-158">If you are presented with more than one tenant ID, carefully select the CSP tenant ID on which you want to receive payments.</span></span> <span data-ttu-id="3030d-159">接下来， **选择"** 确认"以确认公司详细信息正确无误，并且应该对所选的 CSP 租户 ID 进行奖励付款。</span><span class="sxs-lookup"><span data-stu-id="3030d-159">Next, select **Confirm** to acknowledge that your company details are correct, and that the incentive payment should be made to the CSP tenant ID that you selected.</span></span>
 
      <span data-ttu-id="3030d-160">如果状态显示" **已确认**"，则 CSP 租户 ID 的分配已完成，无需进一步操作。</span><span class="sxs-lookup"><span data-stu-id="3030d-160">If the status shows **Confirmed**, the assignment of the CSP tenant ID has been completed and no further action is required.</span></span> <span data-ttu-id="3030d-161">仍可以选择"已确认"以查看分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-161">You may still select Confirmed to see the details of the assignment.</span></span>
   
      <span data-ttu-id="3030d-162">在要求合作伙伴明确请求应用税务豁免的国家/地区，在奖励计划以及位置 MPN 的税务配置文件部分，可以选择应用税务配置文件旁边的税务豁免。</span><span class="sxs-lookup"><span data-stu-id="3030d-162">In countries that require partners  explicitly to request to apply a tax exemption, there will be an option to apply tax exemption next to the tax profile in the tax profile section of the incentive program and location MPN.</span></span> <span data-ttu-id="3030d-163">选中此框将税务豁免权益应用于奖励额度说明。</span><span class="sxs-lookup"><span data-stu-id="3030d-163">Checking this box will apply tax exemption benefits to your incentive credit note.</span></span> 
   
      <span data-ttu-id="3030d-164">目前，LRD 信用额度付款方式仅适用于 Microsoft 商务奖励计划的澳大利亚、新西兰和加拿大合作伙伴。</span><span class="sxs-lookup"><span data-stu-id="3030d-164">Currently, the LRD Credit Note payment method is available only for Australia, New Zealand, and Canada partners for the Microsoft Commerce Incentive program.</span></span> <span data-ttu-id="3030d-165">如果你是注册 MCI 计划的这三个国家/地区中的直接计费合作伙伴或间接提供商，并且未看到 LRD 信用额度作为可用付款方式，请确认租户 ID 与相关合作伙伴 MPN 位置帐户相关联。</span><span class="sxs-lookup"><span data-stu-id="3030d-165">If you’re a direct bill partner or indirect provider in these three countries enrolled for the MCI program and you don’t see LRD credit note as the available payment method, then confirm your tenant ID is associated with the relevant partner MPN location account.</span></span> <span data-ttu-id="3030d-166">有关此内容详细信息， [请阅读如何更新组织配置文件](update-your-partner-profile.md)。</span><span class="sxs-lookup"><span data-stu-id="3030d-166">For more information on this, read [how to update your organization profile](update-your-partner-profile.md).</span></span>

    
5. <span data-ttu-id="3030d-167">选择"**货币"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-167">Select the **Currency**.</span></span>

6. <span data-ttu-id="3030d-168">完成所有付款字段后，选择"提交 **"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-168">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="set-up-a-default-bank-profile"></a><span data-ttu-id="3030d-169">设置默认银行配置文件</span><span class="sxs-lookup"><span data-stu-id="3030d-169">Set up a default bank profile</span></span>

<span data-ttu-id="3030d-170">你可设置默认银行配置文件并将其分配到 MPN 位置。</span><span class="sxs-lookup"><span data-stu-id="3030d-170">You can set up default bank profiles and assign them to MPN locations.</span></span> <span data-ttu-id="3030d-171">Microsoft 将使用这些默认配置文件进行该 MPN 位置的后续注册。</span><span class="sxs-lookup"><span data-stu-id="3030d-171">These defaults profiles will be used by Microsoft for subsequent enrollments for that MPN location.</span></span> 

1. <span data-ttu-id="3030d-172">登录到仪表板[合作伙伴中心，](https://partner.microsoft.com/dashboard/)然后选择齿轮图标以 **打开设置**   菜单。</span><span class="sxs-lookup"><span data-stu-id="3030d-172">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/),  and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="3030d-173">选择 **"帐户设置**"，展开" **付款和税务"** 部分，然后选择" **付款和税务配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-173">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profiles**.</span></span> 

3. <span data-ttu-id="3030d-174">在 **"付款配置文件"部分** 下选择" **管理默认配置文件** "。</span><span class="sxs-lookup"><span data-stu-id="3030d-174">Select **Manage default profiles** under the **Payment profiles** section.</span></span> 

4. <span data-ttu-id="3030d-175">若要创建默认银行配置文件，请选择 **"添加默认银行配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-175">To create a default bank profile, select **Add a default bank profile**.</span></span> 

5. <span data-ttu-id="3030d-176">从公司的可用银行配置文件列表中选择银行配置文件，选择要用于此银行配置文件的货币，然后选择要应用此默认配置文件的 MPN 位置列表。</span><span class="sxs-lookup"><span data-stu-id="3030d-176">Select a bank profile from the list of available bank profiles of your company, select the currency to be used with this bank profile, and then select the list of MPN locations for which you want this default profile to apply.</span></span>

6. <span data-ttu-id="3030d-177">完成 **选择** 后，选择"完成"。</span><span class="sxs-lookup"><span data-stu-id="3030d-177">Select **Done** once you have completed the selections.</span></span> <span data-ttu-id="3030d-178">完成所有必填字段之前，"完成"按钮将不可单击。</span><span class="sxs-lookup"><span data-stu-id="3030d-178">The Done button will not be clickable until all required fields have been completed.</span></span> 

>[!NOTE]
><span data-ttu-id="3030d-179">同一个银行和货币配对可以应用于多个位置。</span><span class="sxs-lookup"><span data-stu-id="3030d-179">The same bank and currency pairing can be applied to multiple locations.</span></span> <span data-ttu-id="3030d-180">如果为位置 MPN 分配了一次默认配置文件和货币组合，则它将不再显示在位置下拉列表中，供将来进行默认配置文件分配。</span><span class="sxs-lookup"><span data-stu-id="3030d-180">If the location MPN has been assigned a default profile and currency combination once, it will no longer appear in the location dropdown for future default profile assignments.</span></span> <span data-ttu-id="3030d-181">如果删除了默认选择，则 MPN 的位置将重新显示，供将来的默认配置文件分配使用。</span><span class="sxs-lookup"><span data-stu-id="3030d-181">If the default selection is deleted, the location MPN will reappear for future default profile assignments.</span></span> <span data-ttu-id="3030d-182">每个银行配置文件和货币组合都作为唯一的可编辑行添加。</span><span class="sxs-lookup"><span data-stu-id="3030d-182">Each bank profile and currency combination is added as an unique, editable row.</span></span>

7. <span data-ttu-id="3030d-183">添加所有必需的更改后，选择"保存 **"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-183">Once all the required changes have been added, select **Save**.</span></span>  

## <a name="create-your-bank-profile"></a><span data-ttu-id="3030d-184">创建银行配置文件</span><span class="sxs-lookup"><span data-stu-id="3030d-184">Create your bank profile</span></span>

<span data-ttu-id="3030d-185">银行配置文件是在公司级别创建的。</span><span class="sxs-lookup"><span data-stu-id="3030d-185">Bank profiles are created at a company level.</span></span> <span data-ttu-id="3030d-186">这允许跨公司内的多个 MPN ID 和奖励计划分配一个银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="3030d-186">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within a company.</span></span> <span data-ttu-id="3030d-187">将银行配置文件应用于不同的国家/地区时，可能会例外，因为不同的银行和税务规则可能适用。</span><span class="sxs-lookup"><span data-stu-id="3030d-187">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="3030d-188">在下列页面上，需要具有星号的字段。</span><span class="sxs-lookup"><span data-stu-id="3030d-188">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="3030d-189">如果不知道字段是什么，请选择信息图标。</span><span class="sxs-lookup"><span data-stu-id="3030d-189">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="3030d-190">在" **详细信息** "页上，填写以下字段： **个人资料名称：** 输入唯一名称以标识此付款配置文件。</span><span class="sxs-lookup"><span data-stu-id="3030d-190">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="3030d-191">**银行帐户位置：** 公司银行所在的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3030d-191">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="3030d-192">**付款方式：** 客户的首选付款方式合作伙伴中心是电子银行转让。</span><span class="sxs-lookup"><span data-stu-id="3030d-192">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="3030d-193">选择“**下一页**”。</span><span class="sxs-lookup"><span data-stu-id="3030d-193">Select **Next**.</span></span>

3. <span data-ttu-id="3030d-194">在" **银行帐户"** 页上，输入你的信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-194">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="3030d-195">此页上显示的字段因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="3030d-195">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="3030d-196">选择“**下一页**”。</span><span class="sxs-lookup"><span data-stu-id="3030d-196">Select **Next**.</span></span>

5. <span data-ttu-id="3030d-197">在 **"位置"** 页上，输入相应的信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-197">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="3030d-198">如果银行需要讨论你的帐户，银行会与你公司联系的人。</span><span class="sxs-lookup"><span data-stu-id="3030d-198">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="3030d-199">填写字段后，选择"完成 **"，** 然后选择" **确认** "以创建银行配置文件。</span><span class="sxs-lookup"><span data-stu-id="3030d-199">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="3030d-200">将重定向到"付款和税务 **配置文件"** 页。</span><span class="sxs-lookup"><span data-stu-id="3030d-200">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="3030d-201">在验证完成之前，新配置文件的状态将反映挂起 **的 Microsoft** 验证。</span><span class="sxs-lookup"><span data-stu-id="3030d-201">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="3030d-202">此过程最多可能需要 48 小时。</span><span class="sxs-lookup"><span data-stu-id="3030d-202">This process may take up to 48 hours.</span></span> <span data-ttu-id="3030d-203">完成验证后，配置文件状态将反映"已批准"**或**"**需要操作"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-203">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="3030d-204">如果需要 **操作**，请重复上述步骤，提供必要的信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-204">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="3030d-205">创建税务配置文件</span><span class="sxs-lookup"><span data-stu-id="3030d-205">Create your tax profile</span></span>

<span data-ttu-id="3030d-206">使用以下过程向 Microsoft 提供组织所需的税务信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-206">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="3030d-207">本部分中的页面是动态的，根据你的国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="3030d-207">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="3030d-208">如需有关识别正确税务信息的帮助，请联系你国家/地区相应的政府来源。</span><span class="sxs-lookup"><span data-stu-id="3030d-208">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="3030d-209">对于北美的合作伙伴公司，如果需要有关填写 W8 或 W9 表单的信息，可以使用以下地址访问 IRS 站点：</span><span class="sxs-lookup"><span data-stu-id="3030d-209">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="3030d-210">仅输入公司的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-210">Enter only details for your company.</span></span> <span data-ttu-id="3030d-211">切勿输入个人详细信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-211">Never enter personal details.</span></span>

1. <span data-ttu-id="3030d-212">在"**业务配置文件"** 页上，填写必填字段，然后选择"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-212">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="3030d-213">在 **"设置** "页上，选择适用于公司的选项。</span><span class="sxs-lookup"><span data-stu-id="3030d-213">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="3030d-214">如果你的公司仅合并到 美国，或者此配置文件适用于个人，请选择左侧的选项。</span><span class="sxs-lookup"><span data-stu-id="3030d-214">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="3030d-215">如果你的公司在公司外部合并，请选择美国，然后从列表中选择你的国家/地区。</span><span class="sxs-lookup"><span data-stu-id="3030d-215">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="3030d-216">选择“**下一页**”。</span><span class="sxs-lookup"><span data-stu-id="3030d-216">Select **Next**.</span></span> 

4. <span data-ttu-id="3030d-217">在"**税务状态"** 页上，输入所需信息，然后选择"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-217">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="3030d-218">此页上的字段因国家/地区而异。</span><span class="sxs-lookup"><span data-stu-id="3030d-218">Fields on this page will vary by country.</span></span> <span data-ttu-id="3030d-219">详细信息。</span><span class="sxs-lookup"><span data-stu-id="3030d-219">your details.</span></span> 

5. <span data-ttu-id="3030d-220">在"**其他文档"** 页上，选择必填字段，然后选择"下一 **步"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-220">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="3030d-221">选择 **"** 浏览"，上传你的国家/地区所需的任何文档。</span><span class="sxs-lookup"><span data-stu-id="3030d-221">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="3030d-222">显示文档名称时，选择 **"Upload"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-222">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="3030d-223">如果需要删除文档，请选择"删除 **"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-223">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="3030d-224">若要保存并继续，请选择"完成 **"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-224">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="3030d-225">在 **弹出** 消息中选择"确认"。</span><span class="sxs-lookup"><span data-stu-id="3030d-225">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="3030d-226">将返回到"付款和税务 **设置"** 页。</span><span class="sxs-lookup"><span data-stu-id="3030d-226">You’ll be taken back to the **Payout and tax setup** page.</span></span>
 
## <a name="update-expired-tax-profiles"></a><span data-ttu-id="3030d-227">更新过期的税务配置文件</span><span class="sxs-lookup"><span data-stu-id="3030d-227">Update expired tax profiles</span></span>

1. <span data-ttu-id="3030d-228">登录到 合作伙伴中心 [仪表板](https://partner.microsoft.com/dashboard/)，然后选择齿轮图标以 **打开设置菜单**。</span><span class="sxs-lookup"><span data-stu-id="3030d-228">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span>

1. <span data-ttu-id="3030d-229">选择 **"帐户设置**"，展开"**付款和税务"** 部分，然后选择"**付款和税务配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-229">Select **Account settings**, expand the **Payout and tax** section, and then select **Payout and tax profile**.</span></span>

1. <span data-ttu-id="3030d-230">选择"**税务配置文件"。**</span><span class="sxs-lookup"><span data-stu-id="3030d-230">Select **Tax profile**.</span></span>

1. <span data-ttu-id="3030d-231">检查" **到期日期"列** 并导航到已过期或即将过期的税务配置文件。</span><span class="sxs-lookup"><span data-stu-id="3030d-231">Check the column **Expiration Date** and navigate to the tax profile that is expired or about to expire.</span></span>

1. <span data-ttu-id="3030d-232">选择“编辑”。</span><span class="sxs-lookup"><span data-stu-id="3030d-232">Select **Edit**.</span></span>

1. <span data-ttu-id="3030d-233">在"税务表单"部分中，通过提供新详细信息来更新税务表单。</span><span class="sxs-lookup"><span data-stu-id="3030d-233">In the tax form section, update the tax forms by providing the new details.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="3030d-234">后续步骤</span><span class="sxs-lookup"><span data-stu-id="3030d-234">Next steps</span></span>

- [<span data-ttu-id="3030d-235">有关付款和税款的常见问题</span><span class="sxs-lookup"><span data-stu-id="3030d-235">Common questions about payouts and taxes</span></span>](payout-faq.yml)
