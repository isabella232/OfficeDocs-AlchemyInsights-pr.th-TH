---
title: การTeamsข้อผิดพลาดการลงชื่อเข้าใช้ AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953060"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>การTeamsข้อผิดพลาดการลงชื่อเข้าใช้ AADSTS9000411

เมื่อลงชื่อเข้าใช้ Microsoft Teams คุณอาจได้รับข้อผิดพลาด: ขออภัย เราพบปัญหาในการลงชื่อเข้าใช้ **AADSTS9000411: การร้องขอไม่ได้รับการจัดรูปแบบอย่างถูกต้อง พารามิเตอร์ "login_hint" จะถูกคัดลอก**

เพื่อแก้ไขปัญหานี้ โปรดตรวจสอบให้แน่ใจว่าไคลเอ็นต์ของคุณMicrosoft Teamsได้รับการอัปเดตแล้ว ดูข้อมูลเพิ่มเติมเกี่ยวกับการอัปเดตลูกค้าของคุณที่[อัปเดตMicrosoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)

ถ้าคุณไม่สามารถอัปเดตไคลเอ็นต์ของคุณด้วยเหตุผลบางอย่าง การบันทึกออกจากไคลเอ็นต์จะล้างข้อมูลที่แคชส่วนใหญ่ อย่างไรก็ตาม ถ้าคุณยังคงมีปัญหาหลังจากออกจากระบบ/เข้าสู่ระบบ ให้ออกจากTeams และโปรดล้างแคชไคลเอ็นต์ของคุณโดยให้ดการดังต่อไปนี้:
1. ปิด Microsoft Teams
2. ไปที่: %appdata%\microsoft\teams แล้วลบไฟล์ทั้งหมด
3. เปิดMicrosoft Teamsอีกครั้ง
