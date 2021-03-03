---
title: การลบข้อมูลและการลบอุปกรณ์จาก Intun1
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
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416332"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>การลบข้อมูลและการลบอุปกรณ์จาก Intun1

การเลิกใช้อุปกรณ์และการล้างอุปกรณ์การล้างอุปกรณ์สามารถใช้เพื่อเอาข้อมูลบริษัทที่จัดการโดย Intun> ออก หรือเพื่อรีเซ็ตเป็นค่าจากโรงงาน และส่งคืนอุปกรณ์เป็นการตั้งค่าเริ่มต้น

1. ลงชื่อเข้าใช้การจัดการอุปกรณ์ Microsoft 365 แล้วไปที่  >  **อุปกรณ์ทั้งหมด**
2. เลือกอุปกรณ์ที่คุณต้องการลบข้อมูล
3. เลือกชนิดของการลบข้อมูลระยะไกลที่คุณต้องการลบ การเลิกใช้จะลบข้อมูลขององค์กรเท่านั้น ในขณะที่การลบข้อมูลทั้งหมดจะคืนค่าอุปกรณ์กลับเป็นการตั้งค่าจากโรงงาน
4. เลือกใช่ เพื่อยืนยัน จนกว่าการลบข้อมูลจะเสร็จสิ้น สถานะการกระบงของอุปกรณ์จะแสดง *เป็น เกษียณที่ค้าง* อยู่
    หลังจากการแอคชันเสร็จสมบูรณ์ คุณจะไม่เห็นอุปกรณ์เคลื่อนที่ในรายการของอุปกรณ์ที่มีการจัดการอีกต่อไป

> [!NOTE]
> ไม่สามารถเอาข้อมูลบริษัทออกจากอุปกรณ์ที่เข้าร่วมไปยัง Azure AD ได้ 

For full details of the effect of the Retired and Wipe actions, including what is retained and what is deleted, see following documentation:

- [ลบอุปกรณ์ออกโดยใช้การลบข้อมูล เลิกใช้ หรือยกเลิกการลงทะเบียนอุปกรณ์](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)ด้วยตนเอง
- [วิธีการลบข้อมูลขององค์กรจากแอป Intun1 ที่มีการจัดการเท่านั้น](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [ลบข้อมูลทั้งหมดจากอุปกรณ์ macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)