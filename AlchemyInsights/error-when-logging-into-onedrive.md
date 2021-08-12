---
title: 0x8004de40การเปิดใช้OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946598"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40การเปิดใช้OneDrive

ถ้าคุณได้รับข้อผิดพลาดเกิดขึ้น **0x8004de40** ลงชื่อเข้าใช้ในOneDrive ให้เริ่มระบบคอมพิวเตอร์ใหม่ขณะที่เชื่อมต่อกับโดเมนที่โรงเรียนหรือที่โรงเรียนของคุณ ถ้าคุณได้รับข้อผิดพลาดนี้หลังจากเริ่มต้นระบบใหม่ ให้ลองวิธีนี้ขณะที่เชื่อมต่อกับโดเมนที่โรงเรียนหรือที่โรงเรียนของคุณ:

1. คลิก เริ่ม แล้วพิมพ์ **cmd** **หรือพร้อมท์**  ของสั่งในกล่องค้นหา คลิกขวาที่แอปพร้อมท์สั่ง  **แล้วเลือก เรียกใช้ในฐานะ** ผู้ดูแลระบบ ถ้าคุณได้รับพร้อมท์ให้ใส่รหัสผ่านผู้ดูแลระบบหรือการยืนยัน ให้พิมพ์รหัสผ่าน หรือ **คลิก** อนุญาต  

2. ในหน้าต่าง พร้อมท์สั่ง ให้พิมพ์ **dsregcmd /leave**  แล้วรอให้สั่งเสร็จสมบูรณ์ จากนั้นพิมพ์ **dsregcmd /join** และรอให้สั่งเสร็จสมบูรณ์
3. เริ่มระบบคอมพิวเตอร์ของคุณใหม่
