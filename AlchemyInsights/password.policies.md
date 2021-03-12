---
title: นโยบายรหัสผ่าน
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
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747055"
---
# <a name="password-policies"></a><span data-ttu-id="356a8-102">นโยบายรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="356a8-102">Password policies</span></span>

<span data-ttu-id="356a8-103">**ฉันมีปัญหากับนโยบายรหัสผ่านของผู้ใช้**</span><span class="sxs-lookup"><span data-stu-id="356a8-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="356a8-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span><span class="sxs-lookup"><span data-stu-id="356a8-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="356a8-105">ระบบคลาวด์เท่านั้นที่ผู้ใช้ต้องเลือกรหัสผ่านที่ตรงตามข้อกฎหมายในบทความนี้: [นโยบายรหัสผ่านที่ใช้กับบัญชีผู้ใช้ระบบคลาวด์เท่านั้น](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="356a8-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="356a8-106">ผู้ใช้ภายในองค์กรต้องเลือกรหัสผ่านที่ตรงกับความต้องการภายในองค์กร</span><span class="sxs-lookup"><span data-stu-id="356a8-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="356a8-107">ถ้าผู้ใช้ภายในองค์กรไม่สามารถตั้งค่ารหัสผ่านได้ ให้ตรวจสอบความต้องการภายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="356a8-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="356a8-108">**ฉันไม่ทราบวิธีการตั้งค่าหรือตรวจสอบนโยบายวันหมดอายุของรหัสผ่าน**</span><span class="sxs-lookup"><span data-stu-id="356a8-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="356a8-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span><span class="sxs-lookup"><span data-stu-id="356a8-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="356a8-110">ให้ปฏิบัติตามคําแนะนํา [ในบทความนี้: ตั้งค่าหรือตรวจสอบนโยบายรหัสผ่านโดยใช้ PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="356a8-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="356a8-111">นโยบายวันหมดอายุของรหัสผ่านของผู้ใช้ภายในองค์กรจะถูกตั้งค่าใน AD ภายในองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="356a8-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="356a8-112">**ลิงก์ที่เป็นประโยชน์อื่นๆ:**</span><span class="sxs-lookup"><span data-stu-id="356a8-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="356a8-113">เริ่มต้นใช้งานการรีเซ็ตรหัสผ่าน</span><span class="sxs-lookup"><span data-stu-id="356a8-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="356a8-114">แก้ไขปัญหาการรีเซ็ตรหัสผ่านที่ผู้ดูแลระบบเริ่ม</span><span class="sxs-lookup"><span data-stu-id="356a8-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
