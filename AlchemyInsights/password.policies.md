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
# <a name="password-policies"></a>นโยบายรหัสผ่าน

**ฉันมีปัญหากับนโยบายรหัสผ่านของผู้ใช้**

- The password policy for a user depends on whether the user is cloud only or on-premises.
- ระบบคลาวด์เท่านั้นที่ผู้ใช้ต้องเลือกรหัสผ่านที่ตรงตามข้อกฎหมายในบทความนี้: [นโยบายรหัสผ่านที่ใช้กับบัญชีผู้ใช้ระบบคลาวด์เท่านั้น](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- ผู้ใช้ภายในองค์กรต้องเลือกรหัสผ่านที่ตรงกับความต้องการภายในองค์กร ถ้าผู้ใช้ภายในองค์กรไม่สามารถตั้งค่ารหัสผ่านได้ ให้ตรวจสอบความต้องการภายในองค์กรของคุณ

**ฉันไม่ทราบวิธีการตั้งค่าหรือตรวจสอบนโยบายวันหมดอายุของรหัสผ่าน**

- You can set and check the expiration policy for cloud users in your tenant by using PowerShell. ให้ปฏิบัติตามคําแนะนํา [ในบทความนี้: ตั้งค่าหรือตรวจสอบนโยบายรหัสผ่านโดยใช้ PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- นโยบายวันหมดอายุของรหัสผ่านของผู้ใช้ภายในองค์กรจะถูกตั้งค่าใน AD ภายในองค์กรของคุณ

**ลิงก์ที่เป็นประโยชน์อื่นๆ:**
- [เริ่มต้นใช้งานการรีเซ็ตรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [แก้ไขปัญหาการรีเซ็ตรหัสผ่านที่ผู้ดูแลระบบเริ่ม](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
