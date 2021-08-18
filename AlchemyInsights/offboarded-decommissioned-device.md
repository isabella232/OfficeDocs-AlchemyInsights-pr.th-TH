---
title: ปัญหาเกี่ยวกับการเอาอุปกรณ์ Offboarded หรืออุปกรณ์ที่ยกเลิกการใช้งานออกจากคลังอุปกรณ์
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324463"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>ปัญหาเกี่ยวกับการเอาอุปกรณ์ Offboarded หรืออุปกรณ์ที่ยกเลิกการใช้งานออกจากคลังอุปกรณ์

ขณะนี้ Microsoft Defender for Endpoint ไม่อนุญาตให้ลบระเบียนอุปกรณ์ของอุปกรณ์ Offboarded หรือยกเลิกการใช้งานด้วยตนเองออกจากคลังอุปกรณ์

เพื่อความปลอดภัย อุปกรณ์จะยังคงอยู่ในพอร์ทัลเป็นระเบียนในอดีตเป็นเวลาถึง 180 วัน อย่างไรก็ตาม ข้อมูลอุปกรณ์จะถูกล้างตามช่วงเวลาการเก็บข้อมูลที่คุณกําหนดค่าไว้

**หมายเหตุ:** อุปกรณ์ Offboarded หรือยกเลิกการใช้งานจะสลับไปยังสถานะ **ไม่ได้ใช้งาน** โดยอัตโนมัติหลังจากผ่านไปเจ็ดวัน นอกจากนี้ อุปกรณ์ที่ไม่ได้ใช้งานใน 30 วันที่ผ่านมาจะไม่นับเป็นข้อมูลที่สะท้อนถึงคะแนนการเปิดรับการจัดการภัยคุกคามและช่องโหว่ที่องค์กรของคุณได้รับหรือคะแนน Microsoft Secure Score for Devices
 
ถ้าคุณยังไม่ต้องการดูอุปกรณ์บางอย่างในมุมมองคลังอุปกรณ์ ให้ลองวางแท็กอุปกรณ์เพื่อกรองอุปกรณ์ที่ยกเลิกจากมุมมองคลังอุปกรณ์

สำหรับข้อมูลเพิ่มเติม ให้ดู:

[อุปกรณ์ Offboard จากบริการ Microsoft Defender for Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[คะแนนแสงในการจัดการภัยคุกคามและช่องโหว่](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[แก้ไขเซนเซอร์ที่ไม่ร้ายแรงใน Microsoft Defender for Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[วิธีใช้การแท็กอย่างมีประสิทธิภาพ (ตอนที่ 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[วิธีใช้การแท็กอย่างมีประสิทธิภาพ (ตอนที่ 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[วิธีใช้การแท็กอย่างมีประสิทธิภาพ (ตอนที่ 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




