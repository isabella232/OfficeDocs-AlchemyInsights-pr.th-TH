---
title: เลื่อนการอัปเกรดทีม
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741790"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>วิธีการเลื่อนการอัปเกรดทีมที่ขับเคลื่อนด้วย Microsoft

**สิ่งสำคัญ**: เราสามารถช่วยแก้ไขปัญหานี้ให้คุณได้โดยใช้การวินิจฉัยการสนับสนุนแต่ดูเหมือนว่าคุณไม่ได้ใช้ศูนย์การจัดการใหม่ เมื่อต้องการใช้ศูนย์การจัดการใหม่ให้เลื่อนตัวสลับที่ด้านบนขวาที่ระบุว่า **ศูนย์การจัดการใหม่** ทางด้านขวา การใช้ศูนย์การจัดการใหม่ให้คลิก **ต้องการความช่วยเหลือ** วิดเจ็ตพิมพ์ "เลื่อนทีมอัปเกรด" แล้วทำตามพร้อมท์เพื่อเรียกใช้การวิเคราะห์การเชื่อมต่อ

ถ้าคุณได้รับการติดต่อสื่อสารเกี่ยวกับการอัปเกรดอัตโนมัติจาก Skype for Business ไปยังทีม Microsoft และคุณต้องการเลื่อนการอัปเกรดอัตโนมัติเป็นวันที่ภายหลังผู้ดูแลระบบส่วนกลางของคุณสามารถลงชื่อเข้าใช้[พอร์ทัลการจัดการทีม](https://admin.teams.microsoft.com/dashboard)และหลังจากเลือกปุ่ม**สถานะการรีเฟรช**ภายใต้การอัปเกรดทีม Microsoft ให้เลือกปุ่ม**เลื่อน** เมื่อต้องการดูวันที่ใหม่สำหรับการอัปเกรดอัตโนมัติของผู้เช่าของคุณไปยังทีม Microsoft ให้รีเฟรชหน้าพอร์ทัลการจัดการทีม

**หมายเหตุ:** ปุ่ม **เลื่อน** จะพร้อมใช้งานก็ต่อเมื่อคุณได้รับการแจ้งเตือนของศูนย์ข้อความเกี่ยวกับการอัปเกรดโดยอัตโนมัติ 

ผู้ดูแลระบบส่วนกลางยังสามารถเรียกใช้ [CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับสถานะการอัปเกรดปัจจุบันของพวกเขาได้
