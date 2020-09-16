---
title: รีเลย์อีเมลผ่าน Microsoft ๓๖๕
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776505"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>ตั้งค่าอุปกรณ์หรือแอปพลิเคชันมัลติฟังก์ชันเพื่อส่งอีเมล

เมื่อต้องการเรียนรู้เกี่ยวกับตัวเลือกของคุณและขั้นตอนต่างๆให้ดูที่[วิธีการตั้งค่าอุปกรณ์แบบมัลติฟังก์ชันหรือแอปพลิเคชันเพื่อส่งอีเมลโดยใช้ Microsoft ๓๖๕](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)
  
**หมายเหตุ:** ถ้าคุณมีอุปกรณ์หรือแอปพลิเคชันที่หยุดทำงานเมื่อเร็วๆนี้โปรดทราบว่าเราได้เริ่ม [การปิดใช้งานการเข้ารหัสการลงจุด](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) ตามแผน เมื่อต้องการดูอุปกรณ์ที่ได้รับผลกระทบให้ไปที่ [รายงานของไคลเอ็นต์การรับรอง](https://protection.office.com/mailflow/dashboard)ความถูกต้องของ SMTP ข้อผิดพลาดทั่วไปอาจคล้ายกับ: ความล้มเหลวในการรับรองความถูกต้อง/ข้อผิดพลาด TLS ล้มเหลว/ข้อผิดพลาดของอัลกอริทึมการเข้ารหัสข้อผิดพลาดของอัลกอริทึมไม่ตรงกัน เมื่อต้องการแก้ไขปัญหาให้ใช้วิธีต่อไปนี้

 - **Windows Server ๒๐๐๓ IIS SMTP จะไม่ทำงานอีกต่อไป–จำเป็นต้องใช้ Windows เวอร์ชันที่ใหม่กว่า**  
 - โปรดตรวจสอบกับแอปพลิเคชันหรือผู้จำหน่ายอุปกรณ์ของคุณเพื่อดูว่าการเข้ารหัสที่ทันสมัยได้รับการสนับสนุนหรือไม่หรือถ้ามีการอัปเดต
