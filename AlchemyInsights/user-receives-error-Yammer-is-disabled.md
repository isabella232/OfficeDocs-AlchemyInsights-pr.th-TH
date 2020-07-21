---
title: ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198369"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>ผู้ใช้ได้รับข้อผิดพลาด AADSTS7000112 Yammer ถูกปิดใช้งาน

ถ้าคุณได้รับข้อผิดพลาด "AADSTS7000112: แอพลิเคชัน '00000005-0000-0ff1-ce000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000005", ปัญหาที่มีอยู่กับบริการหลักภายในโฆษณา Azure ผู้ดูแลระบบอาจปิดใช้งานบริการหลักเพื่อบล็อกการเข้าถึง Yammer

การปิดใช้งานบริการหลักไม่แนะนํา และอาจทําให้เกิดปัญหาเพิ่มเติม สําหรับข้อมูลเพิ่มเติมเกี่ยวกับวิธีการที่ได้รับการสนับสนุนเพื่อบล็อกการเข้าถึงของผู้ใช้ไปยัง Yammer ให้ดูที่[ปิดการเข้าถึง Yammer สําหรับผู้ใช้ Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)  

เมื่อต้องการแก้ไขปัญหานี้ในเว็บไซต์ Azure และคืนค่าการเข้าถึงของผู้ใช้ไปยัง Yammer:

1.  เปิดหน้าไดเรกทอรีที่ใช้งานอยู่ของ Azure และเลือก**โปรแกรมประยุกต์องค์กร**ภายใต้**จัดการ**ในบานหน้าต่างด้านซ้าย
3.  พิมพ์**Office 365 Yammer**ในกล่องค้นหา และเลือกชื่อโปรแกรมประยุกต์เพื่อเปิดการตั้งค่า
4.  เลือก**คุณสมบัติ**ภายใต้**จัดการ**ในบานหน้าต่างการนําทางด้านซ้าย
5.  ตั้งค่าของ**เปิดใช้งานสําหรับผู้ใช้เพื่อลงชื่อเข้าใช้หรือไม่**เป็น**ใช่**แล้วเลือก**บันทึก**
6.  ลงชื่อเข้าใช้ Yammer อีกครั้ง คุณอาจต้องล้างคุกกี้

อีกวิธีหนึ่งคือ เรียกใช้คําสั่ง PowerShell เพื่อตั้งค่า สําหรับข้อมูลเพิ่มเติม ให้ดูที่["ขออภัย แต่เรากําลังมีปัญหาในการลงชื่อเข้าใช้คุณ"](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365) 