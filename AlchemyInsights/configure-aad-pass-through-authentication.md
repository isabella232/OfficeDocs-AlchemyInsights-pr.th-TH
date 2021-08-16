---
title: กําหนดAzure Active Directoryการรับรองความถูกต้องแบบพาส-through
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
ms.openlocfilehash: 9ac9ba7b469e523fd12c22fcf07a3944603dc6665e82fce4df329a257ac87ca4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978756"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a>กําหนดAzure Active Directoryการรับรองความถูกต้องแบบพาส-through

ต่อไปนี้เป็นคู่มือบางส่วนเพื่อช่วยให้คุณกําหนดค่าการรับรองความถูกต้องแบบพาส-ผ่าน:

- **เมื่อต้องการตั้งค่าการAzure Active Directory เชื่อมต่อ**: คู่มือ [การซิงค์ผู้ใช้กับไดเรกทอรี](https://admin.microsoft.com/AdminPortal/Home)ของคุณจะช่วยให้คุณกําหนดค่าการซิงโครไนซ์แฮชของรหัสผ่านหรือการรับรองความถูกต้องแบบพาส-ผ่าน การกําหนดค่านี้ช่วยให้ผู้ใช้สามารถลงชื่อเข้าใช้อีเมลของพวกเขาและ Active Directory (ตัวควบคุมโดเมน) ภายในองค์กรของคุณโดยใช้รหัสผ่านเดียวกันได้  การซิงค์ [ผู้ใช้กับคู่มือไดเรกทอรีของคุณ](https://admin.microsoft.com/AdminPortal/Home) ยังครอบคลุมการลงชื่อเข้าใช้การติดต่อกับภายนอกด้วย Active Directory Federation Services (AD FS) ด้วย

- **เมื่อต้องการตั้งค่าฟีเจอร์ Azure:** คู่มือการตั้งค่า [Azure AD](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup)จะแนะAzure Active Directoryการตั้งค่าฟีเจอร์ใน Azure Active Directory Basic เช่น การจัดการการเข้าถึงแบบกลุ่ม การตั้งค่ารหัสผ่านใหม่แบบบริการตนเองของแอประบบคลาวด์ และพร็อกซีแอปพลิเคชัน Azure Active Directory เพื่อเผยแพร่เว็บแอปภายในองค์กร


