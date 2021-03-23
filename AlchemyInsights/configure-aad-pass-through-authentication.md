---
title: กําหนดค่าการรับรองความถูกต้องแบบพาส-ทะลุผ่านของ Azure Active Directory
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037533"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a>กําหนดค่าการรับรองความถูกต้องแบบพาส-ทะลุผ่านของ Azure Active Directory

ต่อไปนี้เป็นแนวทางบางส่วนเพื่อช่วยให้คุณกําหนดค่าการรับรองความถูกต้องแบบพาส-ผ่าน:

- **เมื่อต้องการตั้งค่า Azure Active Directory Connect**: การซิงค์ผู้ใช้กับ [คู่มือ](https://admin.microsoft.com/AdminPortal/Home) ไดเรกทอรีของคุณจะช่วยให้คุณกําหนดค่าการซิงโครไนซ์แฮชของรหัสผ่านหรือการรับรองความถูกต้องแบบพาส-ผ่าน การกําหนดค่านี้จะให้ผู้ใช้ลงชื่อเข้าใช้อีเมลของพวกเขาและ Active Directory (ตัวควบคุมโดเมน) ภายในองค์กรของคุณโดยใช้รหัสผ่านเดียวกัน  การซิงค์ [ผู้ใช้กับคู่มือไดเรกทอรีของคุณ](https://admin.microsoft.com/AdminPortal/Home) ยังครอบคลุมถึงการลงชื่อเข้าใช้การติดต่อกับภายนอกด้วย Active Directory Federation Services (AD FS) ด้วย

- เมื่อต้องการตั้งค่าฟีเจอร์ **Azure:** คู่มือการตั้งค่า [Azure AD](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup)จะแนะนเกี่ยวกับการตั้งค่าฟีเจอร์ใน Azure Active Directory Basic เช่น การจัดการการเข้าถึงแบบกลุ่ม การตั้งค่ารหัสผ่านใหม่แบบบริการตนเองของแอประบบคลาวด์ และพร็อกซีแอปพลิเคชัน Azure Active Directory เพื่อเผยแพร่เว็บแอปภายในองค์กร


