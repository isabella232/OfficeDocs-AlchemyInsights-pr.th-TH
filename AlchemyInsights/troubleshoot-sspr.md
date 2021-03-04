---
title: แก้ไขปัญหา SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430212"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="31aaa-102">แก้ไขปัญหา SSPR</span><span class="sxs-lookup"><span data-stu-id="31aaa-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="31aaa-103">**ฉันมีปัญหาในการกําหนดค่าการรีเซ็ตรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="31aaa-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="31aaa-104">ถ้าคุณเป็นผู้ดูแลระบบและค้นหาวิธีการเปิดใช้งานการตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง ให้ดู [บทช่วยสอนเปิดใช้งาน SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)เพื่อกําหนดค่าการตั้งค่ารหัสผ่านใหม่ให้กับองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="31aaa-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="31aaa-105">คุณยังอาจต้องการตรวจสอบข้อ [ควรทราบด้าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="31aaa-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="31aaa-106">คุณต้องได้รับมอบหมายสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="31aaa-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="31aaa-107">**ระบบคลาวด์เฉพาะผู้ใช้** - Office 365 (O365) ชําระเงิน SKU หรือ Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="31aaa-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="31aaa-108">**ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ในองค์กร** - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="31aaa-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="31aaa-109">หากมีข้อสงสัยเพิ่มเติมเกี่ยวกับการรีเซ็ตรหัสผ่านด้วยตนเอง โปรดดู FAQ[ของเรา](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="31aaa-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="31aaa-110">**ฉันได้รับข้อความแสดงข้อผิดพลาด**</span><span class="sxs-lookup"><span data-stu-id="31aaa-110">**I'm getting an error message**</span></span>

<span data-ttu-id="31aaa-111">ตรวจทานบทความนี้เพื่อค้นหาข้อผิดพลาดทั่วไปและโซลูชัน: แก้ไขปัญหา [การตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="31aaa-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="31aaa-112">**ฉันมีปัญหากับนโยบายการตั้งค่ารหัสผ่านใหม่ของฉัน**</span><span class="sxs-lookup"><span data-stu-id="31aaa-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="31aaa-113">ถ้านโยบายรีเซ็ตรหัสผ่านของคุณไม่เป็นไปตามที่คาดไว้ หรือถ้าคุณมีข้อถามเกี่ยวกับนโยบายรีเซ็ตรหัสผ่าน ให้อ่านบทความนี้: นโยบายและข้อจํากัดของรหัสผ่าน[ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="31aaa-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="31aaa-114">นโยบายการตั้งค่ารหัสผ่านใหม่จะไม่ใช้กับผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="31aaa-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="31aaa-115">Microsoft บังคับใช้นโยบายรีเซ็ตรหัสผ่านสองทางเริ่มต้นอย่างรัดกุมให้กับบทบาทผู้ดูแลระบบ Azure</span><span class="sxs-lookup"><span data-stu-id="31aaa-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="31aaa-116">ตรวจสอบให้แน่ใจว่าคุณได้ทดสอบกับผู้ใช้ที่ไม่ใช่ผู้ดูแลระบบ</span><span class="sxs-lookup"><span data-stu-id="31aaa-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="31aaa-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="31aaa-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="31aaa-118">**ฉันไม่ต้องการให้ผู้ใช้ลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติมเพื่อตั้งค่ารหัสผ่านใหม่**</span><span class="sxs-lookup"><span data-stu-id="31aaa-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="31aaa-119">คุณสามารถใส่ข้อมูลล่วงหน้า (แอตทริบิวต์อีเมลและโทรศัพท์) ให้กับผู้ใช้ของคุณโดยใช้ API, PowerShell หรือ Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="31aaa-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="31aaa-120">เมื่อต้องการเรียนรู้วิธีอ่าน:</span><span class="sxs-lookup"><span data-stu-id="31aaa-120">To learn how read:</span></span>

- [<span data-ttu-id="31aaa-121">การปรับใช้การรีเซ็ตรหัสผ่านโดยไม่ให้ผู้ใช้ลงทะเบียน</span><span class="sxs-lookup"><span data-stu-id="31aaa-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="31aaa-122">การรีเซ็ตรหัสผ่านจะใช้ข้อมูลใด</span><span class="sxs-lookup"><span data-stu-id="31aaa-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="31aaa-123">**ฉันต้องการให้ผู้ใช้ของฉันลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติมของพวกเขาในการตั้งค่ารหัสผ่านใหม่**</span><span class="sxs-lookup"><span data-stu-id="31aaa-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="31aaa-124">ให้ผู้ใช้ของคุณลงทะเบียนข้อมูลความปลอดภัยของพวกเขาเพื่อรีเซ็ตรหัสผ่านด้วยตนเองโดยให้[ส่งaka.ms/ssprsetupให้พวกเขา](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="31aaa-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="31aaa-125">หลังจากใส่ข้อมูลให้กับผู้ใช้ (โดยผู้ใช้หรือผู้ดูแลระบบ) ให้มอบสิทธิ์ผู้ใช้ของคุณในการaka.ms/ssprเพื่อให้ผู้ใช้สามารถตั้งค่ารหัสผ่าน[](https://passwordreset.microsoftonline.com/)ของพวกเขาใหม่ได้</span><span class="sxs-lookup"><span data-stu-id="31aaa-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="31aaa-126">If users are still experiencing problems they are mostly **federrated** or **password hash synch** users.</span><span class="sxs-lookup"><span data-stu-id="31aaa-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="31aaa-127">ซึ่งหมายความว่าอาจมีปัญหากับบริการ Password Writeback</span><span class="sxs-lookup"><span data-stu-id="31aaa-127">This means there is likely a problem with the Password Writeback service.</span></span>