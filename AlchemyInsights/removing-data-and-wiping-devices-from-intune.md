---
title: การเอาข้อมูลออกและการลบอุปกรณ์ออกจาก Intun1
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922281"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>การเอาข้อมูลออกและการลบอุปกรณ์ออกจาก Intun1

การเลิกใช้อุปกรณ์และการล้างข้อมูลอุปกรณ์การล้างอุปกรณ์สามารถใช้เพื่อเอาข้อมูลบริษัทที่จัดการโดย Intun1 ออก หรือเพื่อรีเซ็ตเป็นค่าจากโรงงาน และส่งคืนอุปกรณ์เป็นการตั้งค่าเริ่มต้น

1. ลงชื่อเข้าใช้Microsoft 365การจัดการอุปกรณ์ และ **ไปที่**  >  **อุปกรณ์ทั้งหมด**
2. เลือกอุปกรณ์ที่คุณต้องการลบข้อมูล
3. เลือกชนิดของการลบข้อมูลระยะไกลที่คุณต้องการลบ การเลิกใช้จะลบข้อมูลขององค์กรเท่านั้น ในขณะที่การลบข้อมูลทั้งหมดจะคืนค่าอุปกรณ์เป็นการตั้งค่าจากโรงงาน
4. เลือกใช่ เพื่อยืนยัน จนกว่าการลบข้อมูลจะเสร็จสิ้น สถานะการกระทบของอุปกรณ์จะแสดงเป็น *เลิกใช้ค้าง* อยู่
    หลังจากการแอคชันเสร็จสมบูรณ์ คุณจะไม่เห็นอุปกรณ์เคลื่อนที่ในรายการของอุปกรณ์ที่มีการจัดการอีกต่อไป

> [!NOTE]
> ไม่สามารถเอาข้อมูลบริษัทออกจากอุปกรณ์ที่เข้าร่วมกับ Azure AD ได้ 

ดูรายละเอียดทั้งหมดของผลกระทบของการเลิกใช้และการล้าง รวมถึงสิ่งที่ถูกเก็บรักษาไว้และสิ่งที่ถูกลบ ให้ดูเอกสารต่อไปนี้:

- [ลบอุปกรณ์ออกโดยใช้ การลบ ข้อมูลการเลิก](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)ใช้ หรือยกเลิกการลงทะเบียนอุปกรณ์ด้วยตนเอง
- [วิธีการลบข้อมูลขององค์กรจากแอปที่มีการจัดการ Intun1 เท่านั้น](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [ลบข้อมูลทั้งหมดจากอุปกรณ์ macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)