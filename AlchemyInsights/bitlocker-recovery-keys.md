---
title: คีย์การกู้คืน Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 8708ed76f6abe81582823c8af89db8fffef9a3c5
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505087"
---
# <a name="accessing-bitlocker-recovery-keys"></a>การเข้าถึงคีย์การกู้คืน Bitlocker

เมื่อกําหนดการตั้งค่า Bitlocker Intuned Endpoint Protection Policy คุณจะสามารถกําหนดได้ว่าควรจัดเก็บข้อมูลการกู้คืน Bitlocker ใน Azure Active Directory หรือไม่

ถ้ามีการกําหนดค่าการตั้งค่าดังกล่าว ผู้ดูแลระบบ Intun1 ควรมองเห็นข้อมูลการกู้คืนที่เก็บไว้โดยเป็นส่วนหนึ่งของข้อมูลระเบียนอุปกรณ์ในอุปกรณ์ Intuns blade ด้วยสองวิธี:

อุปกรณ์ - อุปกรณ์ Azure AD -> "อุปกรณ์" หรือ ->อุปกรณ์ทั้งหมด -> "อุปกรณ์" ->คีย์การกู้คืน

อีกวิธีหนึ่งคือ ถ้ามีการเข้าถึงแบบผู้ดูแลระบบไปยังอุปกรณ์ นั้น สามารถมองเห็นคีย์การกู้คืน (รหัสผ่าน) โดยการเรียกใช้การสั่งต่อไปนี้จากพร้อมท์สั่งผู้ดูแล:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
ถ้าอุปกรณ์ถูกเข้ารหัสลับก่อนการลงทะเบียน intuned คีย์การกู้คืนอาจเชื่อมโยงกับ "บัญชี Microsoft" (MSA) ที่ใช้ในการลงชื่อเข้าใช้อุปกรณ์ในระหว่างกระบวนการ OOBE ถ้าเป็นกรณีนี้ การเข้าถึง  https://onedrive.live.com/recoverykey และการลงชื่อเข้าใช้ด้วย MSA ควรแสดงอุปกรณ์ที่จัดเก็บคีย์การกู้คืนไว้
 
ถ้าอุปกรณ์ถูกเข้ารหัสลับเนื่องจากผลลัพธ์ของการกําหนดค่าผ่านนโยบายกลุ่มที่ยึดตามโดเมน ข้อมูลการกู้คืนอาจถูกจัดเก็บไว้ใน Active Directory ภายในองค์กร

ถ้าคุณได้กําหนดค่านโยบายการป้องกันจุดสิ้นสุดเพื่อจัดเก็บคีย์การกู้คืนใน Azure Active Directory แต่ยังไม่ได้อัปโหลดคีย์บนอุปกรณ์ที่ระบุ คุณสามารถทริกเกอร์การอัปโหลดโดยการหมุนคีย์การกู้คืนของอุปกรณ์นั้นจากคอนโซล MEM For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).

