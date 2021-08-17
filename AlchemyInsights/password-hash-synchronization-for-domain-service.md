---
title: การซิงโครไนซ์แฮชของรหัสผ่านของบริการโดเมน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040885"
---
# <a name="password-hash-synchronization-for-domain-service"></a>การซิงโครไนซ์แฮชของรหัสผ่านของบริการโดเมน

**ถ้าอินสแตนซ์ Azure AD DS ของคุณพร้อมท์ให้คุณเปิดใช้งานการซิงโครไนซ์แฮชของรหัสผ่าน**

คุณพบกับสถานการณ์สมมติที่คุณเรียกใช้สภาพแวดล้อมแบบไฮบริดกับผู้ใช้ซิงโครไนซ์จากสภาพแวดล้อม Domain Services (AD DS) Azure Active Directoryภายในองค์กร สถานการณ์นี้จะถูกพบแม้คุณจะมีการซิงโครไนซ์แฮชรหัสผ่านจาก AD DS ภายในองค์กรไปยังผู้เช่า Azure AD ของคุณ

**สาเหตุ**

ปัญหานี้เกิดขึ้นเนื่องจากการตั้งค่า Azure AD เชื่อมต่อจะไม่ซิงโครไนซ์ตัวจัดการ LAN ทางเทคโนโลยีใหม่ (NTLM) และ Hashes รหัสผ่าน Kerberos ที่ต้องใช้กับ Azure AD DS

**วิธีแก้ไขปัญหาชั่วคราว** 

คุณจะต้องกําหนดค่ารหัสผ่าน Azure AD เชื่อมต่อซิงโครไนซ์รหัสผ่านที่ต้องใช้ในการรับรองความถูกต้องของ NTLM และ Kerberos

หลังจากกําหนดเชื่อมต่อ Azure AD แล้ว การสร้างบัญชีภายในองค์กรหรือเหตุการณ์การเปลี่ยนรหัสผ่านจะซิงโครไนซ์ Hashe รหัสผ่านเดิมกับ Azure AD ด้วย โปรดดูที่นี่ [สําหรับ](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) ข้อมูลเพิ่มเติมเกี่ยวกับสิ่งนี้และสําหรับแนวทางเกี่ยวกับวิธีการเปิดใช้งานการซิงโครไนซ์รหัสผ่านในสภาพแวดล้อมไฮบริดของ Azure AD DS