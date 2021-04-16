---
title: เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814283"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน

**อาการ**

ผู้ใช้ไม่สามารถเปิดรายงานได้ "มีบางอย่างผิดพลาด ตรวจสอบรายละเอียดด้านเทคนิคเพื่อดูรายละเอียดเพิ่มเติม"

**สาเหตุ**

รายงานไม่สามารถโหลดใน UCI ที่มีข้อผิดพลาด "Form descriptor เป็น null หรือไม่ได้กําหนด" รายงานใน UCI ยังต้องใช้กล่องโต้ตอบแบบดั้งเดิม ดังนั้นระบบของลูกค้าต้อง *เปิดใช้งาน allowlegacydialogsembeม*

**วิธีแก้ไข**

1. ไปที่ การตั้งค่า **>การดูแล> การตั้งค่า> บนแท็บ** ทั่วไป

2. ตั้งค่า "เปิดใช้งานการฝังของกล่องโต้ตอบดั้งเดิมบางรายการในไคลเอ็นต์เบราว์เซอร์ส่วนติดต่อแบบรวม" **เป็น** ใช่
