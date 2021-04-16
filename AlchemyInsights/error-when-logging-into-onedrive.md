---
title: 0x8004de40เปิด OneDrive
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813671"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40เปิด OneDrive

ถ้าคุณได้รับข้อผิดพลาดเกี่ยวกับ **0x8004de40** เมื่อลงชื่อเข้าใช้ OneDrive ให้เริ่มระบบคอมพิวเตอร์ใหม่ขณะที่เชื่อมต่อกับโดเมนที่โรงเรียนหรือที่โรงเรียนของคุณ ถ้าคุณได้รับข้อผิดพลาดนี้หลังจากเริ่มต้นระบบใหม่ ให้ลองวิธีนี้ขณะที่เชื่อมต่อกับโดเมนที่โรงเรียนหรือที่โรงเรียนของคุณ:

1. คลิก เริ่ม แล้วพิมพ์ **cmd** **หรือพร้อมท์**  ของสั่งในกล่องค้นหา คลิกขวาที่แอปพร้อมท์สั่ง  **แล้วเลือก เรียกใช้ในฐานะ** ผู้ดูแลระบบ ถ้าคุณได้รับพร้อมท์ให้ใส่รหัสผ่านผู้ดูแลระบบหรือการยืนยัน ให้พิมพ์รหัสผ่าน หรือ **คลิก** อนุญาต  

2. ในหน้าต่าง พร้อมท์สั่ง ให้พิมพ์ **dsregcmd /leave**  แล้วรอให้สั่งเสร็จสมบูรณ์ จากนั้นพิมพ์ **dsregcmd /join** และรอให้สั่งเสร็จสมบูรณ์
3. เริ่มระบบคอมพิวเตอร์ของคุณใหม่
