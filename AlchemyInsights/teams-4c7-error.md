---
title: ข้อผิดพลาด Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786688"
---
# <a name="4c7-error-in-microsoft-teams"></a>ข้อผิดพลาด 4c7 ใน Microsoft Teams

ข้อผิดพลาดนี้เกิดขึ้นเนื่องจาก Microsoft Teams ต้องใช้การรับรองความถูกต้องของฟอร์ม เมื่อคุณปรับใช้ Active Directory Federation Services (AD FS) การรับรองความถูกต้องของฟอร์มจะไม่เปิดใช้งานกับอินทราเน็ตตามค่าเริ่มต้น ถ้าการรับรองความถูกต้องของแบบรวมของ Windows ล้มเหลว คุณจะได้รับพร้อมท์ให้ลงชื่อเข้าใช้โดยใช้การรับรองความถูกต้องของฟอร์ม

เมื่อต้องการแก้ไขปัญหานี้ ให้เปิดใช้งานการรับรองความถูกต้องของฟอร์มโดยใช้ Snap-in ของ AD FS Microsoft Management Console (MMC) บนคอมพิวเตอร์ที่มีสําเนาภายในเครื่องของ Active Directory เมื่อต้องการให้ปฏิบัติตามขั้นตอนเหล่านี้: 

1. ในบานหน้าต่างนําทาง ให้เรียกดู **นโยบายการรับรองความถูกต้อง**
2. ภายใต้ **การ** แอคชัน ในบานหน้าต่างรายละเอียด ให้เลือก แก้ไข **การรับรองความถูกต้องหลัก** ส่วนกลาง
3. บนแท็บ **อินทราเน็ต ให้เลือก****การรับรองความถูกต้องของฟอร์ม**
4. เลือก **ตกลง** (หรือ **Apply**)