---
title: เลื่อนTeamsอัปเกรด
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
ms.openlocfilehash: 893a01ae74f8aec9bb0079430188e3cd6881b3009818830ea5572cfa41cdf71f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923996"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a>วิธีการเลื่อนการอัปเกรดที่ขับเคลื่อนโดย Microsoft Teams

**สิ่ง** สําคัญ: เราสามารถช่วยแก้ไขปัญหานี้ให้คุณโดยใช้การวินิจฉัยการสนับสนุน แต่ดูเหมือนว่าคุณไม่ได้ใช้ศูนย์การจัดการใหม่ เมื่อต้องการใช้ศูนย์การจัดการใหม่ เลื่อนตัวสลับที่ด้านบนขวาที่ระบุว่า **ศูนย์การจัดการ** ใหม่ ไปทางขวา ใช้ศูนย์การจัดการใหม่ คลิกวิดเจ็ต **ต้องการ** ความช่วยเหลือหรือไม่ พิมพ์ "เลื่อนTeamsอัปเกรด" แล้วปฏิบัติตามพร้อมท์เพื่อเรียกใช้การวินิจฉัย

ถ้าคุณได้รับการติดต่อสื่อสารเกี่ยวกับการอัปเกรดอัตโนมัติที่ขับเคลื่อนโดยไมโครซอฟท์จาก Skype for Business เป็น Microsoft Teams และคุณต้องการเลื่อนการอัปเกรดอัตโนมัติเป็นวันที่ใหม่กว่า ผู้ดูแลระบบส่วนกลางของคุณสามารถเข้าสู่ระบบพอร์ทัลผู้ดูแลระบบ[Teams](https://admin.teams.microsoft.com/dashboard)และหลังจากเลือกปุ่ม สถานะการรีเฟรช ภายใต้ อัปเกรด Microsoft Teams ให้เลือกปุ่ม เลื่อนออกไป เมื่อต้องการดูวันที่ใหม่ให้อัปเกรดโดยอัตโนมัติของผู้เช่าMicrosoft Teamsของคุณ ให้รีเฟรชTeamsพอร์ทัลผู้ดูแลระบบของคุณ

**หมายเหตุ:** **ปุ่ม เลื่อน** ออกไป จะพร้อมใช้งานถ้าคุณได้รับการแจ้งเตือนจากศูนย์ข้อความเกี่ยวกับการอัปเกรดอัตโนมัติเท่านั้น 

ผู้ดูแลระบบส่วนกลางยังสามารถเรียกใช้ [Get-CsTeamsUpgraderStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) เพื่อเรียนรู้เพิ่มเติมเกี่ยวกับสถานะการอัปเกรดปัจจุบันของพวกเขาได้
