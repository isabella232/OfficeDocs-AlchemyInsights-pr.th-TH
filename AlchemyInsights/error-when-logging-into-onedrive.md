---
title: ข้อผิดพลาด0x8004de40 เมื่อเปิดใช้งาน OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823120"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>ข้อผิดพลาด0x8004de40 เมื่อเปิดใช้งาน OneDrive

ถ้าคุณได้รับข้อผิดพลาด **0x8004de40** เมื่อเข้าสู่ระบบ OneDrive ให้รีบูตเครื่องคอมพิวเตอร์ในขณะที่เชื่อมต่อกับโดเมนของที่ทำงานหรือที่โรงเรียนของคุณ ถ้าคุณได้รับข้อผิดพลาดนี้หลังจากรีบูตให้ลองใช้วิธีนี้ในขณะที่เชื่อมต่อกับโดเมนของที่ทำงานหรือโรงเรียนของคุณ:

1. คลิกเริ่มแล้วพิมพ์ **cmd** หรือ **พร้อมท์คำสั่ง** ในกล่องค้นหาให้คลิกขวาบนแอปพร้อมท์คำสั่งแล้วเลือก **เรียกใช้ในฐานะผู้ดูแลระบบ** ถ้าคุณได้รับพร้อมท์สำหรับรหัสผ่านผู้ดูแลระบบหรือการยืนยันให้พิมพ์รหัสผ่านหรือคลิก **อนุญาต**  

2. ในหน้าต่างพร้อมท์คำสั่งให้พิมพ์ **dsregcmd/leave**  และรอให้คำสั่งเสร็จสมบูรณ์ จากนั้นพิมพ์ **dsregcmd/join** และรอให้คำสั่งเสร็จสมบูรณ์
3. เริ่มต้นระบบคอมพิวเตอร์ของคุณใหม่
