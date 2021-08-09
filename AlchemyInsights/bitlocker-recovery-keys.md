---
title: คีย์การกู้คืน Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060083"
---
# <a name="accessing-bitlocker-recovery-keys"></a>การเข้าถึงคีย์การกู้คืน Bitlocker

เมื่อกําหนดการตั้งค่า Bitlocker นโยบายการป้องกันจุดสิ้นสุด Intuned คุณจะสามารถกําหนดได้ว่าข้อมูลการกู้คืน Bitlocker ควรถูกจัดเก็บAzure Active Directoryหรือไม่

ถ้าการตั้งค่าดังกล่าวได้รับการกําหนดค่า ผู้ดูแลระบบ Intun1 ควรเห็นข้อมูลการกู้คืนที่เก็บไว้โดยเป็นส่วนหนึ่งของข้อมูลระเบียนอุปกรณ์ในอุปกรณ์ Intuns blade ด้วยสองวิธี:

อุปกรณ์ - อุปกรณ์ Azure AD -> "อุปกรณ์" หรืออุปกรณ์ ->อุปกรณ์ทั้งหมด -> "อุปกรณ์" ->คีย์การกู้คืน

อีกวิธีหนึ่งคือ ถ้ามีการเข้าถึงแบบผู้ดูแลระบบไปยังอุปกรณ์ นั้น สามารถดูคีย์การกู้คืน (รหัสผ่าน) ได้โดยการเรียกใช้การสั่งต่อไปนี้จากพร้อมท์สั่งที่ยกระดับ:

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
ถ้าอุปกรณ์ถูกเข้ารหัสลับก่อน enrolment intuned คีย์การกู้คืนอาจเชื่อมโยงกับ "บัญชี Microsoft" (MSA) ที่ใช้ในการลงชื่อเข้าใช้อุปกรณ์ในระหว่างกระบวนการ OOBE ถ้าเป็นกรณีนี้ การเข้าถึงและการ  https://onedrive.live.com/recoverykey ลงชื่อเข้าใช้ด้วย MSA ควรแสดงอุปกรณ์ที่จัดเก็บคีย์การกู้คืนไว้
 
ถ้าอุปกรณ์ถูกเข้ารหัสลับเป็นผลลัพธ์ของการกําหนดค่าผ่านนโยบายกลุ่มที่ใช้โดเมน ข้อมูลการกู้คืนอาจถูกเก็บไว้ใน Active Directory ภายในองค์กร

ถ้าคุณได้กําหนดค่านโยบายการป้องกันจุดสิ้นสุดเพื่อจัดเก็บคีย์การกู้คืนใน Azure Active Directory แต่ยังไม่ได้อัปโหลดคีย์ของอุปกรณ์ที่ระบุ คุณสามารถทริกเกอร์การอัปโหลดโดยการหมุนคีย์การกู้คืนของอุปกรณ์นั้นจากคอนโซล MEM โปรดดูรายละเอียดที่[หมุนคีย์การกู้คืน BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

