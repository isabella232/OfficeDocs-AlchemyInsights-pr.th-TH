---
title: แก้ไขข้อผิดพลาดการลงชื่อเข้าใช้ Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822006"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>แก้ไขข้อผิดพลาดการลงชื่อเข้าใช้ Teams AADSTS9000411

เมื่อลงชื่อเข้าใช้ Microsoft Teams คุณอาจได้รับข้อผิดพลาด: ขออภัย เราพบปัญหาในการลงชื่อเข้าใช้ **AADSTS9000411: ไม่สามารถจัดรูปแบบการร้องขอได้อย่างถูกต้อง พารามิเตอร์ "login_hint" จะถูกคัดลอก**

เมื่อต้องการแก้ไขปัญหานี้ โปรดตรวจสอบให้แน่ใจว่าลูกค้า Microsoft Teams ของคุณได้รับการอัปเดตแล้ว ดูข้อมูลเพิ่มเติมเกี่ยวกับการอัปเดตลูกค้าของคุณที่[อัปเดต Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

ถ้าคุณไม่สามารถอัปเดตไคลเอ็นต์ของคุณด้วยเหตุผลบางอย่าง การบันทึกออกจากไคลเอ็นต์จะล้างข้อมูลที่แคชส่วนใหญ่ อย่างไรก็ตาม ถ้าคุณยังคงมีปัญหาหลังจากออกจาก Logoff/logon ให้ออกจาก Teams และโปรดล้างแคชไคลเอ็นต์ของคุณโดยวิธีการต่อไปนี้:
1. ปิด Microsoft Teams
2. ไปที่: %appdata%\microsoft\teams แล้วลบไฟล์ทั้งหมด
3. เปิด Microsoft Teams อีกครั้ง
