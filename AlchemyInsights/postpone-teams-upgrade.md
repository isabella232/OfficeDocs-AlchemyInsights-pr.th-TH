---
title: เลื่อนการอัปเกรด Teams ออกไป
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801250"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>วิธีการเลื่อนการอัปเกรด Microsoft-Driven Teams

**สิ่ง** สําคัญ: เราสามารถช่วยแก้ไขปัญหานี้ให้คุณโดยใช้การวินิจฉัยการสนับสนุน แต่ดูเหมือนว่าคุณไม่ได้ใช้ศูนย์การจัดการใหม่ เมื่อต้องการใช้ศูนย์การจัดการใหม่ เลื่อนตัวสลับที่ด้านบนขวาที่ระบุว่า **ศูนย์การจัดการ** ใหม่ ไปทางขวา ใช้ศูนย์การจัดการใหม่ คลิกวิดเจ็ต **ต้องการ** ความช่วยเหลือหรือไม่ พิมพ์ "เลื่อนการอัปเกรด Teams" แล้วตามพร้อมท์เพื่อเรียกใช้การวินิจฉัย

หากคุณได้รับการติดต่อสื่อสารเกี่ยวกับการอัปเกรดอัตโนมัติจาก Skype for Business จาก Microsoft for Business ไปยัง Microsoft Teams และคุณต้องการเลื่อนการอัปเกรดอัตโนมัติออกไปในภายหลัง ผู้ดูแลระบบส่วนกลางของคุณสามารถเข้าสู่ระบบพอร์ทัลผู้ดูแลระบบ[ของ Teams](https://admin.teams.microsoft.com/dashboard)และหลังจากเลือกปุ่มรีเฟรชสถานะ ภายใต้การอัปเกรด Microsoft Teamsให้เลือกปุ่ม เลื่อนออกไป เมื่อต้องการดูวันที่ใหม่ในการอัปเกรดอัตโนมัติของผู้เช่าของคุณไปยัง Microsoft Teams ให้รีเฟรชหน้าพอร์ทัลการดูแลระบบ Teams

**หมายเหตุ:** **ปุ่ม เลื่อน** ออกไป จะพร้อมใช้งานถ้าคุณได้รับการแจ้งเตือนจากศูนย์ข้อความเกี่ยวกับการอัปเกรดอัตโนมัติเท่านั้น 

ผู้ดูแลระบบส่วนกลางยังสามารถเรียกใช้ [Get-CsTeamsUpgraderStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับสถานะการอัปเกรดปัจจุบันของพวกเขาได้
