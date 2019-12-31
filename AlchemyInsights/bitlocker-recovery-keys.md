---
title: คีย์การกู้คืน Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908833"
---
# <a name="accessing-bitlocker-recovery-keys"></a>การเข้าถึงคีย์การกู้คืน Bitlocker

เมื่อกำหนดค่า Bitlocker นโยบายการป้องกันปลายทาง Intune คุณสามารถกำหนดว่าข้อมูลการกู้คืน Bitlocker ควรถูกเก็บไว้ในไดเรกทอรีที่ใช้งานอยู่ของ Azure หรือไม่

ถ้าการตั้งค่าถูกกำหนดค่าข้อมูลการกู้คืนที่เก็บไว้ควรจะมองเห็นได้กับผู้ดูแลระบบ Intune เป็นส่วนหนึ่งของข้อมูลบันทึกอุปกรณ์ในใบมีดอุปกรณ์ Intune ในสองวิธี:

อุปกรณ์-อุปกรณ์ Azure โฆษณา-> "อุปกรณ์" หรืออุปกรณ์-> ทั้งหมดอุปกรณ์-> "อุปกรณ์"-> การกู้คืนคีย์

อีกวิธีหนึ่งคือถ้ามีการเข้าถึงระดับผู้ดูแลไปยังอุปกรณ์ตัวเองคีย์การกู้คืน (รหัสผ่าน) สามารถมองเห็นได้โดยการเรียกใช้คำสั่งต่อไปนี้จากพร้อมท์คำสั่ง:

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
ถ้าอุปกรณ์ถูกเข้ารหัสลับก่อนการลงทะเบียนใน Intune คีย์การกู้คืนอาจมีการเชื่อมโยงกับ "บัญชี Microsoft" (MSA) ที่ใช้ในการเข้าสู่ระบบไปยังอุปกรณ์ในระหว่างกระบวนการ OOBE หากเป็นกรณีนี้การเข้าถึงhttps://onedrive.live.com/recoverykeyและการลงชื่อเข้าใช้ด้วย MSA นั้นควรแสดงอุปกรณ์ที่เก็บคีย์การกู้คืนไว้
 
ถ้าอุปกรณ์ถูกเข้ารหัสเป็นผลมาจากการกำหนดค่าผ่านนโยบายกลุ่มโดเมนข้อมูลการกู้คืนอาจถูกเก็บไว้ในไดเรกทอรีที่ใช้งานอยู่ในสถานที่
 

