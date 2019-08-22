---
title: แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525078"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive

ถ้าคุณได้รับข้อผิดพลาด 0x8004de40 OneDrive:

- รีบูตเครื่องคอมพิวเตอร์ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมนของไดเรกทอรี Acitve ของคุณ
- ถ้ามีการเริ่มระบบไม่สามารถแก้ไขปัญหา unjoin และข้อมูลอุปกรณ์ของคุณจากโฆษณา Azure 

**หมายเหตุ**: คุณควรบนเครือข่ายขององค์กรของคุณในขณะที่กำลังดำเนินการขั้นตอนเหล่านี้ ไม่ต้องทำขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรของคุณ (ตัวอย่างเช่น ระหว่างการเดินทาง) 

- เปิดพร้อมท์คำสั่ง 
- เมื่อต้องการเปิดพร้อมท์คำสั่ง คลิ ก -**เริ่ม**คลิกขวาที่**หน้าจอพร้อมรับคำสั่ง**และ แล้ว คลิก**เรียกใช้ในฐานะผู้ดูแล**
- พิมพ์*dsregcmd /leave*และกด**Enter**
- เมื่อเสร็จสิ้น พิมพ์*dsregcmd /join*และกด**Enter**
- เมื่อเสร็จสิ้น ปิดพรอมต์คำสั่ง
- รีบูตเครื่องคอมพิวเตอร์ และเข้าสู่ระบบไปยัง OneDrive