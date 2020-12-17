---
title: 使用多重身份验证来设置用户
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: 了解如何为员工设置 MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578282"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="0ab98-103">使用多重身份验证来设置用户</span><span class="sxs-lookup"><span data-stu-id="0ab98-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="0ab98-104">**相应的角色**</span><span class="sxs-lookup"><span data-stu-id="0ab98-104">**Appropriate roles**</span></span>

- <span data-ttu-id="0ab98-105">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0ab98-105">Global admin</span></span>

<span data-ttu-id="0ab98-106">增强隐私保护和安全性是我们优先关注的事项。</span><span class="sxs-lookup"><span data-stu-id="0ab98-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="0ab98-107">我们知道，最好的防御措施是防患于未然，链条的强度取决于其最弱的一环。</span><span class="sxs-lookup"><span data-stu-id="0ab98-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="0ab98-108">因此，我们需要生态系统中的所有人都行动起来，确保将安全保护措施实施到位。</span><span class="sxs-lookup"><span data-stu-id="0ab98-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="0ab98-109">强烈建议所有合作伙伴为其合作伙伴租户中的用户启用多重身份验证 (MFA)。</span><span class="sxs-lookup"><span data-stu-id="0ab98-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="0ab98-110">为用户添加多重身份验证</span><span class="sxs-lookup"><span data-stu-id="0ab98-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="0ab98-111">必须具有公司的全局管理员身份才能完成此任务。</span><span class="sxs-lookup"><span data-stu-id="0ab98-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="0ab98-112">为用户启用 MFA 的最简单方法是将用户添加到 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="0ab98-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="0ab98-113">登录 [Azure 门户](https://portal.azure.com)，然后转到“用户管理”。</span><span class="sxs-lookup"><span data-stu-id="0ab98-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="0ab98-114">选择“多重身份验证”。</span><span class="sxs-lookup"><span data-stu-id="0ab98-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="0ab98-115">选择要启用的用户，然后选择“启用”。</span><span class="sxs-lookup"><span data-stu-id="0ab98-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="0ab98-116">这可为此用户启用 MFA。</span><span class="sxs-lookup"><span data-stu-id="0ab98-116">This will enable MFA for this user.</span></span> <span data-ttu-id="0ab98-117">“已启用”表示用户首次登录时，系统会要求其设置自己的 MFA 验证。</span><span class="sxs-lookup"><span data-stu-id="0ab98-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="0ab98-118">此后，这些用户在登录时需要提供通过电子邮件或短信（取决于其具体设置）收到的代码。</span><span class="sxs-lookup"><span data-stu-id="0ab98-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="指定如何验证":::

>[!NOTE]
><span data-ttu-id="0ab98-120">可以强制用户使用 MFA，方法是使用与上面相同的步骤，并选择“强制执行” 。</span><span class="sxs-lookup"><span data-stu-id="0ab98-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="0ab98-121">若要了解详细信息，请参阅[启用每用户 Azure 多重身份验证来保护登录事件](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates)。</span><span class="sxs-lookup"><span data-stu-id="0ab98-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="0ab98-122">所有用户的初始状态都为“已禁用” \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="0ab98-122">All users start out **Disabled**.</span></span> <span data-ttu-id="0ab98-123">将用户注册到每用户 Azure 多重身份验证中后，用户状态更改为“已启用” \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="0ab98-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="0ab98-124">当已启用的用户登录并完成注册过程后，其状态更改为“已强制执行” \*\*\*\* 。</span><span class="sxs-lookup"><span data-stu-id="0ab98-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="0ab98-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="0ab98-125">Next steps</span></span>

- [<span data-ttu-id="0ab98-126">向用户分配角色和权限</span><span class="sxs-lookup"><span data-stu-id="0ab98-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

