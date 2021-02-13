---
title: เพิ่ม Microsoft Edge ไปยัง Microsoft Intun1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194578"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a>เพิ่ม Microsoft Edge ไปยัง Microsoft Intun1

เพื่อให้สามารถปรับใช้ กําหนดค่า ตรวจสอบ และปกป้อง Microsoft Edge for Windows 10 ได้ คุณต้องเพิ่ม Microsoft Intuned ก่อน

> [!IMPORTANT]
- Intun1 สนับสนุน Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่า
- Intuned จะตรวจหาการติดตั้ง Microsoft Edge ที่มีอยู่ก่อน
- ถ้า Microsoft Edge ถูกติดตั้งในบริบทของผู้ใช้ การติดตั้งระบบจะเขียนทับการติดตั้งในบริบทของผู้ใช้
- ถ้า Microsoft Edge ได้รับการติดตั้งในบริบทของระบบ ระบบจะรายงานความสเร็จในการติดตั้ง
- Microsoft Edge 77 และเวอร์ชันที่ใหม่กว่าที่ติดตั้งไว้ล่วงหน้าในแชนเนลทั้งหมดในบริบทของผู้ใช้จะถูกเขียนทับด้วย Microsoft Edge ที่ติดตั้งในบริบทของระบบ

**เงื่อนไขเบื้องต้น**

Windows 10 เวอร์ชัน 1709 หรือเวอร์ชันที่ใหม่กว่า

**ขั้นตอนในการเพิ่ม Edge ไปยัง Intuned**

1. [กําหนดค่าแอปใน Intun>](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
2. [กําหนดค่าข้อมูล](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป
3. [กําหนดค่าการตั้งค่า](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป
4. [เลือกแท็กขอบเขต (ไม่บังคับ)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)
5. [เพิ่ม](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)แอป

หากต้องการความช่วยเหลือเพิ่มเติม [โปรดดู](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)การแก้ไขปัญหา




