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
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794224"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>ปัญหาด้านประสิทธิภาพการ Microsoft Defender for Endpoint บน Linux

บทความนี้จะแนะแนวคุณผ่านขั้นตอนในการระบุปัญหาด้านประสิทธิภาพการแต่ละอย่างของ Microsoft Defender for Endpoint บน Linux

สิ่งสําคัญคือต้องตรวจสอบก่อนว่าปัญหาที่คุณพบได้รับการแก้ไขด้วย[เวอร์ชันล่าสุด](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

เมื่อต้องการเริ่มการตรวจสอบ ให้ดู แก้ไขปัญหา[ประสิทธิภาพการโยกย้าย Microsoft Defender for Endpoint บน Linux](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>การยกเว้น

การยกเว้นสามารถช่วยบรรเทาปัญหาด้านประสิทธิภาพการช่วยได้ ตรวจสอบข้อยกเว้นของคุณก่อนที่คุณจะเริ่มต้น เพื่อให้ทราบและทราบความเสี่ยงเพิ่มเติม

For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).

เมื่อคุณมีหลายไฟล์&โฟลเดอร์ที่ไม่ต้องการและทั้งหมดอยู่ในที่ยึดเดียวกัน การยกเว้นที่ยึดอาจง่ายกว่า เริ่มต้นด้วยรุ่นเดือนกุมภาพันธ์ 101.22.80 คุณไม่สามารถยกเว้นจุดยึดทั้งหมดได้

ตัวอย่างเช่น ถ้า /mnt/backup เป็น mountpoint คุณสามารถเพิ่ม /mnt/backup ลงในรายการแยกโดยการเรียกใช้การสั่งนี้:

`$ mdatp exclusion folder add –path /mnt/backup`

**หมายเหตุ**: การเพิ่มการยกเว้นจะมีความเสี่ยงต่อมัลแวร์ที่จะไม่ถูกตรวจพบและควรได้รับการจัดการและดําเนินการด้วยความระมัดระวัง

## <a name="need-help"></a>ต้องการความช่วยเหลือหรือไม่

เพื่อช่วยคุณอย่างมีประสิทธิภาพสูงสุด ให้รวบรวมข้อมูลการวินิจฉัยก่อนที่จะเปิดกรณีสนับสนุน
