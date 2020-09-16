---
title: แก้ไขข้อผิดพลาด0x8004de40 ใน OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745149"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>แก้ไขข้อผิดพลาด0x8004de40 ใน OneDrive

ถ้าคุณได้รับข้อผิดพลาด0x8004de40 กับ OneDrive:

- รีบูตเครื่องคอมพิวเตอร์ที่ได้รับผลกระทบในขณะที่เชื่อมต่อกับโดเมนไดเรกทอรี Acitve ของคุณ
- ถ้าการรีบูทไม่สามารถแก้ไขปัญหาได้ให้เลิกและเข้าร่วมอุปกรณ์ของคุณจาก Azure AD 

**หมายเหตุ**: คุณควรอยู่บนเครือข่ายขององค์กรของคุณในขณะที่ดำเนินการขั้นตอนเหล่านี้ อย่าทำตามขั้นตอนเหล่านี้เมื่อคุณไม่สามารถเชื่อมต่อกับโครงสร้างพื้นฐานขององค์กรของคุณ (ตัวอย่างเช่นในขณะเดินทาง) 

- เปิดพร้อมท์คำสั่งยกระดับ 
- เมื่อต้องการเปิดพร้อมท์คำสั่งยกระดับให้คลิก-**เริ่ม**แล้วคลิกขวาที่**พร้อมท์คำสั่ง**แล้วคลิก**เรียกใช้ในฐานะผู้ดูแลระบบ**
- พิมพ์*dsregcmd/leave*แล้วกด**Enter**
- เมื่อทำเสร็จแล้วให้พิมพ์*dsregcmd/join*แล้วกด**Enter**
- เมื่อทำเสร็จแล้วให้ปิดพร้อมท์คำสั่ง
- รีบูตเครื่องคอมพิวเตอร์แล้วเข้าสู่ระบบ OneDrive