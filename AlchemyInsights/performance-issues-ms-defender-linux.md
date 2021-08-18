---
title: ปัญหาด้านประสิทธิภาพการ Microsoft Defender for Endpoint บน Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: ab6ad888b34524ac6e3b3d5448d0e6be409ffc0e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331876"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>ปัญหาด้านประสิทธิภาพการ Microsoft Defender for Endpoint บน Linux

บทความนี้จะแนะแนวคุณผ่านขั้นตอนในการระบุปัญหาด้านประสิทธิภาพการแต่ละอย่างของ Microsoft Defender for Endpoint บน Linux

สิ่งสําคัญคือต้องตรวจสอบก่อนว่าปัญหาที่คุณพบได้รับการแก้ไขด้วย[เวอร์ชันล่าสุด](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-whatsnew) 

เมื่อต้องการเริ่มการตรวจสอบ ให้ดู แก้ไขปัญหา[ประสิทธิภาพการโยกย้าย Microsoft Defender for Endpoint บน Linux](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>การยกเว้น

การยกเว้นสามารถช่วยบรรเทาปัญหาด้านประสิทธิภาพการช่วยได้ ตรวจสอบข้อยกเว้นของคุณก่อนที่คุณจะเริ่มต้น เพื่อให้ทราบและทราบความเสี่ยงเพิ่มเติม

For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/linux-exclusions).

เมื่อคุณมีหลายไฟล์&โฟลเดอร์ที่ไม่ต้องการและทั้งหมดอยู่ในที่ยึดเดียวกัน อาจง่ายกว่าหากไม่รวมที่ยึด เริ่มต้นด้วยรุ่นเดือนกุมภาพันธ์ 101.22.80 คุณไม่สามารถยกเว้นจุดยึดทั้งหมดได้

ตัวอย่างเช่น ถ้า /mnt/backup เป็น mountpoint คุณสามารถเพิ่ม /mnt/backup ลงในรายการแยกโดยการเรียกใช้การสั่งนี้:

`$ mdatp exclusion folder add –path /mnt/backup`

**หมายเหตุ**: การเพิ่มการยกเว้นจะมีความเสี่ยงต่อมัลแวร์ที่จะไม่ถูกตรวจพบและควรได้รับการจัดการและดําเนินการด้วยความระมัดระวัง

## <a name="need-help"></a>ต้องการความช่วยเหลือหรือไม่

เพื่อช่วยคุณอย่างมีประสิทธิภาพสูงสุด ให้รวบรวมข้อมูลการวินิจฉัยก่อนที่จะเปิดกรณีสนับสนุน
