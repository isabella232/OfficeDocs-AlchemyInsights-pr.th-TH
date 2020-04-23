---
title: แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716047"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>แก้ไขข้อผิดพลาด 0x8004de40 ใน OneDrive

ถ้าคุณได้รับข้อผิดพลาด 0x8004de40 ด้วย OneDrive:

- รีบูตเครื่องคอมพิวเตอร์ที่ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมนไดเรกทอรี Acitve ของคุณ
- ถ้าการเริ่มระบบใหม่ไม่สามารถแก้ไขปัญหา ให้ยกเลิกเข้าร่วม และเข้าร่วมอุปกรณ์ของคุณจาก Azure AD อีกครั้ง 

**หมายเหตุ**: คุณควรอยู่ในเครือข่ายองค์กรของคุณในขณะที่ทําตามขั้นตอนเหล่านี้ อย่าทําตามขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรได้ (เช่น ขณะเดินทาง) 

- เปิดพร้อมท์คําสั่ง 
- เมื่อต้องการเปิดพร้อมท์คําสั่ง ให้คลิก -**เริ่ม**คลิกขวาที่**พร้อมท์คําสั่ง**แล้วคลิก**เรียกใช้ในฐานะผู้ดูแลระบบ**
- พิมพ์*dsregcmd /leave*และกด**Enter**
- เมื่อเสร็จสมบูรณ์*dsregcmd /join***Enter**
- เมื่อเสร็จสิ้น ให้ปิดพรอมต์คําสั่ง
- รีบูตเครื่องคอมพิวเตอร์ และเข้าสู่ระบบ OneDrive