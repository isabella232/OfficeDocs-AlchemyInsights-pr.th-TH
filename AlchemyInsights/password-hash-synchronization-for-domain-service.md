---
title: การซิงโครไนซ์แฮชของรหัสผ่านกับบริการโดเมน
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
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177619"
---
# <a name="password-hash-synchronization-for-domain-service"></a>การซิงโครไนซ์แฮชของรหัสผ่านกับบริการโดเมน

**ถ้าอินสแตนซ์ Azure AD DS ของคุณพร้อมท์ให้คุณเปิดใช้งานการซิงโครไนซ์แฮชของรหัสผ่าน**

คุณพบกับสถานการณ์สมมติที่คุณเรียกใช้สภาพแวดล้อมแบบไฮบริดกับผู้ใช้ที่ซิงโครไนซ์จากสภาพแวดล้อม Azure Active Directory Domain Services (AD DS) ภายในองค์กร สถานการณ์นี้จะพบแม้คุณจะมีการซิงโครไนซ์แฮชรหัสผ่านจาก AD DS ภายในองค์กรไปยังผู้เช่า Azure AD ของคุณ

**สาเหตุ**

ปัญหานี้เกิดขึ้นเนื่องจาก Azure AD Connect ตามค่าเริ่มต้นจะไม่ซิงโครไนซ์ Hashes ของ Technology LAN แบบดั้งเดิม (NTLM) และ Kerberos Password Hashes ที่ต้องใช้ใน Azure AD DS

**วิธีแก้ไขปัญหาชั่วคราว** 

คุณจะต้องกําหนดค่า Azure AD Connect เพื่อซิงโครไนซ์ Hashes รหัสผ่านที่ต้องใช้ในการรับรองความถูกต้องของ NTLM และ Kerberos

หลังจากกําหนดค่า Azure AD Connect แล้ว การสร้างบัญชีภายในองค์กรหรือเหตุการณ์การเปลี่ยนรหัสผ่านจะซิงโครไนซ์ Hashe ของรหัสผ่านดั้งเดิมกับ Azure AD ด้วย โปรดดู [ที่นี่](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) สําหรับข้อมูลเพิ่มเติมเกี่ยวกับสิ่งนี้และสําหรับแนวทางเกี่ยวกับวิธีการเปิดใช้งานการซิงโครไนซ์รหัสผ่านในสภาพแวดล้อมแบบไฮบริดของ Azure AD DS