---
title: เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204678"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>เปิดใช้งานการฝังกล่องโต้ตอบแบบดั้งเดิมเพื่อเปิดรายงาน

**อาการ**

ผู้ใช้ไม่สามารถเปิดรายงานได้ "มีบางอย่างผิดปกติ ตรวจสอบรายละเอียดทางเทคนิคสําหรับรายละเอียดเพิ่มเติม"

**สาเหตุ**

รายงานจะล้มเหลวในการโหลดใน UCI มีข้อผิดพลาด "ตัวบอกลักษณะแบบฟอร์มเป็น null หรือไม่ได้กําหนด" รายงานใน UCI ยังคงต้องการกล่องโต้ตอบแบบดั้งเดิม ดังนั้นระบบของลูกค้าจึงจําเป็นต้องเปิดใช้งาน*allowlegacydialogsembedding*

**โซลูชัน**

1. ไปที่**การตั้งค่า>การจัดการ> > แท็บ ทั่วไป**

2. ตั้งค่า "เปิดใช้งานการฝังกล่องโต้ตอบดั้งเดิมบางอย่างในไคลเอ็นต์เบราว์เซอร์ส่วนติดต่อแบบรวม" เป็น**ใช่**
