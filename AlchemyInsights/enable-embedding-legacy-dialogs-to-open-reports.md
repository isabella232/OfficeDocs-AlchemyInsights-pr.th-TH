---
title: เปิดใช้งานกล่องโต้ตอบการฝังแบบดั้งเดิมเพื่อเปิดรายงาน
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
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806454"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>เปิดใช้งานกล่องโต้ตอบการฝังแบบดั้งเดิมเพื่อเปิดรายงาน

**อาการ**

ผู้ใช้ไม่สามารถเปิดรายงานได้ "มีบางอย่างผิดพลาด ตรวจสอบรายละเอียดทางเทคนิคสำหรับรายละเอียดเพิ่มเติม "

**สาเหตุ**

รายงานจะล้มเหลวในการโหลดใน UCI ที่มีข้อผิดพลาด "ตัวอธิบายฟอร์มเป็น null หรือไม่ได้กำหนดไว้" รายงานใน UCI ยังจำเป็นต้องมีกล่องโต้ตอบแบบดั้งเดิมดังนั้นระบบของลูกค้าจึงจำเป็นต้องมีการเปิดใช้งาน*allowlegacydialogsembedding*

**วิธีแก้ไข**

1. ไปที่การ**ตั้งค่า >การตั้งค่าระบบ > การดูแลระบบ > แท็บทั่วไป**

2. ตั้งค่า "เปิดใช้งานการฝังของกล่องโต้ตอบแบบดั้งเดิมบางรายการในไคลเอ็นต์เบราว์เซอร์ส่วนติดต่อ" เป็น**ใช่**
