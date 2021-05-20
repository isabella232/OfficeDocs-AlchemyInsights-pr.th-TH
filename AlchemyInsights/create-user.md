---
title: สร้างผู้ใช้
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569766"
---
# <a name="create-user"></a><span data-ttu-id="57847-102">สร้างผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="57847-102">Create user</span></span>

<span data-ttu-id="57847-103">**ประกาศ:**</span><span class="sxs-lookup"><span data-stu-id="57847-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="57847-104">[การเลิกใช้การสนับสนุนการลงชื่อเข้าใช้ WebView จาก Google ตั้งแต่วันที่ 4 มกราคม 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="57847-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="57847-105">ทดสอบว่าแอปของคุณอาจได้รับผลกระทบจากแนวทาง [ของ Google เกี่ยวกับ](https://go.microsoft.com/fwlink/?linkid=2157323) การทดสอบความเข้ากันได้หรือไม่</span><span class="sxs-lookup"><span data-stu-id="57847-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="57847-106">ตรวจสอบให้แน่ใจว่าคุณใช้มุมมองเว็บของระบบหรือเบราว์เซอร์ระบบเมื่อลงชื่อเข้าใช้ผู้ใช้ของคุณด้วยบัญชี Google ของลูกค้า</span><span class="sxs-lookup"><span data-stu-id="57847-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="57847-107">For more information, [see Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span><span class="sxs-lookup"><span data-stu-id="57847-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="57847-108">**ฉันไม่สามารถสร้างผู้ใช้ใหม่ในไดเรกทอรี Azure AD ของฉัน**</span><span class="sxs-lookup"><span data-stu-id="57847-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="57847-109">ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้สร้างผู้ใช้มาตรฐานใหม่</span><span class="sxs-lookup"><span data-stu-id="57847-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="57847-110">เฉพาะผู้ดูแลระบบส่วนกลางหรือบทบาทผู้ดูแลระบบผู้ใช้ใน Azure Active Directory (AD) เท่านั้นที่สามารถสร้างผู้ใช้มาตรฐานใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="57847-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="57847-111">ถ้าคุณไม่ได้อยู่ในบทบาทใดบทบาทหนึ่ง ให้ขอให้ผู้ดูแลระบบเพิ่มคุณลงในบทบาทเหล่านี้ หรือสร้างบัญชีผู้ใช้ใหม่ให้คุณ</span><span class="sxs-lookup"><span data-stu-id="57847-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="57847-112">ตรวจสอบให้แน่ใจว่าชื่อผู้ใช้อยู่ในโดเมนที่ได้รับการยืนยันใน Azure AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="57847-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="57847-113">ถ้าคุณไม่มีชื่อโดเมนแบบปรับแต่งเองที่ตรวจสอบแล้วใน Azure AD คุณสามารถใช้โดเมนเริ่มต้น Azure AD ของคุณ ซึ่งลงท้ายด้วย \*.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="57847-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="57847-114">ตรวจสอบให้แน่ใจว่าชื่อผู้ใช้อยู่ในโดเมนที่ไม่ได้ติดต่อกับภายนอก Azure AD จาก AD ภายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="57847-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="57847-115">ผู้ใช้ไม่สามารถเพิ่มในระบบคลาวด์ด้วยชื่อโดเมนที่ติดต่อกับภายนอกจากภายในองค์กรได้</span><span class="sxs-lookup"><span data-stu-id="57847-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="57847-116">ตรวจสอบให้แน่ใจว่าไม่มีผู้ใช้หรือที่ติดต่ออื่นมีชื่อผู้ใช้ที่คุณต้องการกําหนดให้กับผู้ใช้ใหม่แล้ว</span><span class="sxs-lookup"><span data-stu-id="57847-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="57847-117">ชื่อผู้ใช้ต้องไม่ซ.ก. ใน Azure AD</span><span class="sxs-lookup"><span data-stu-id="57847-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="57847-118">ดู [บทบาทและผู้ดูแลระบบ Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) ของ Azure AD</span><span class="sxs-lookup"><span data-stu-id="57847-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="57847-119">ดู [ชื่อโดเมนของ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD ของคุณ</span><span class="sxs-lookup"><span data-stu-id="57847-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="57847-120">ตรวจทาน [บันทึก](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) การตรวจสอบเพื่อดูข้อมูลโดยละเอียดเพิ่มเติมเกี่ยวกับผู้ใช้ที่สร้างหรือผู้ใช้ที่ถูกลบเมื่อเร็วๆ นี้ เช่น ผู้ที่เป็นผู้ปฏิบัติการและเมื่อใด</span><span class="sxs-lookup"><span data-stu-id="57847-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="57847-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="57847-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="57847-122">[บทบาทผู้ดูแลระบบ Azure AD](/azure/active-directory/active-directory-assign-admin-roles): สิทธิ์บทบาทผู้ดูแลระบบในAzure Active Directory</span><span class="sxs-lookup"><span data-stu-id="57847-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="57847-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span><span class="sxs-lookup"><span data-stu-id="57847-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
