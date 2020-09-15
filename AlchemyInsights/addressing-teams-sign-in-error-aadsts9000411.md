---
title: การกำหนดความผิดพลาดในการลงชื่อเข้าใช้ในทีม AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687057"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>การกำหนดความผิดพลาดในการลงชื่อเข้าใช้ในทีม AADSTS9000411

เมื่อคุณลงชื่อเข้าใช้ Microsoft team คุณอาจได้รับข้อผิดพลาด: **ขออภัยแต่เรากำลังมีปัญหาเกี่ยวกับการลงชื่อเข้าใช้คุณใน AADSTS9000411: การร้องขอจะไม่ถูกจัดรูปแบบอย่างถูกต้อง พารามิเตอร์ "login_hint" จะซ้ำกัน**

เมื่อต้องการแก้ปัญหานี้โปรดตรวจสอบให้แน่ใจว่าไคลเอ็นต์ Microsoft team ของคุณได้รับการอัปเดต สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการอัปเดตลูกค้าของคุณให้ดูที่[อัปเดต Microsoft ทีม](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

ถ้าคุณไม่สามารถอัปเดตไคลเอ็นต์ของคุณได้ด้วยเหตุผลบางประการการออกจากระบบไคลเอ็นต์จะล้างข้อมูลที่แคชไว้ที่สุด อย่างไรก็ตามถ้าคุณยังคงมีปัญหาหลังจากออกจากระบบ/เข้าสู่ระบบออกจากทีมและโปรดล้างแคชของไคลเอ็นต์ของคุณโดยทำดังต่อไปนี้:
1. ปิดทีม Microsoft
2. ไปที่:%appdata%\microsoft\teams และลบไฟล์ทั้งหมด
3. เปิดทีม Microsoft อีกครั้ง
