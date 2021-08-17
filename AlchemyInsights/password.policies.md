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
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040849"
---
# <a name="password-policies"></a>นโยบายรหัสผ่าน

**ฉันมีปัญหากับนโยบายรหัสผ่านของผู้ใช้**

- นโยบายรหัสผ่านของผู้ใช้จะขึ้นอยู่กับว่าผู้ใช้ใช้ Cloud เท่านั้นหรือภายในองค์กร
- Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- ผู้ใช้ภายในองค์กรต้องเลือกรหัสผ่านที่ตรงตามข้อกฎหมายภายในองค์กร ถ้าผู้ใช้ภายในองค์กรไม่สามารถตั้งค่ารหัสผ่านของพวกเขา ให้ตรวจสอบความต้องการภายในองค์กรของคุณ

**ฉันไม่ทราบวิธีการตั้งค่าหรือตรวจสอบนโยบายการหมดอายุของรหัสผ่าน**

- You can set and check the expiration policy for cloud users in your tenant by using PowerShell. Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- นโยบายวันหมดอายุของรหัสผ่านของผู้ใช้ภายในองค์กรจะถูกตั้งค่าใน AD ภายในองค์กรของคุณ

**ลิงก์ที่เป็นประโยชน์อื่นๆ:**
- [เริ่มต้นใช้งานการรีเซ็ตรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [แก้ไขปัญหาการรีเซ็ตรหัสผ่านที่ผู้ดูแลระบบเริ่ม](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
