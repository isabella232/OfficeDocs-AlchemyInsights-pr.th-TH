---
title: โปรไฟล์ Wi-Fi แบบ Intun
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555816"
---
# <a name="intune-wi-fi-profiles"></a>โปรไฟล์ Wi-Fi แบบ Intun

การดําเนินการที่ประสบความสําเร็จของการเชื่อมต่อ Wi-Fi สําหรับไคลเอนต์ MDM ขึ้นอยู่กับโปรไฟล์ที่ใช้งานอย่างถูกต้องซึ่งสะท้อนถึงความต้องการของโครงสร้างพื้นฐาน Wi-Fi ขององค์กร ในการตรวจสอบการตั้งค่าที่เหมาะสมสําหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกําลังตรวจสอบ โปรดดู: 

[เพิ่มการตั้งค่า Wi-Fi สําหรับอุปกรณ์ที่ใช้ Android ใน Microsoft Intun](https://docs.microsoft.com/intune/wi-fi-settings-android)

[เพิ่มการตั้งค่า Wi-Fi สําหรับอุปกรณ์ Android องค์กรที่ทุ่มเทและมีการจัดการอย่างเต็มที่ใน Microsoft Intun](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[เพิ่มการตั้งค่า Wi-Fi สําหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intuni](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[เพิ่มการตั้งค่า Wi-Fi สําหรับ Windows 10 และอุปกรณ์ที่ใหม่กว่าใน Intun](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[นําเข้าการตั้งค่า Wi-Fi สําหรับอุปกรณ์ Windows ใน Intun](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**ปัญหาทั่วไป**

**ฉันกําลังปรับใช้โพรไฟล์ Wi-Fi ที่ขึ้นอยู่กับใบรับรองที่ปรับใช้ซึ่งระบุไว้ในโปรไฟล์ Wi-Fi อย่างไรก็ตาม โปรไฟล์การตั้งค่าคอนฟิกจะแสดงสถานะข้อผิดพลาด**

ตรวจสอบว่าอุปกรณ์ของคุณได้รับใบรับรอง

1. ใน Intun เยือกไปที่**อุปกรณ์ทั้งหมด**และเลือกอุปกรณ์>**การกําหนดค่าอุปกรณ์**

2. ตรวจสอบว่า โพรไฟล์ที่คาดว่าจะทั้งหมดจะแสดงรายการ และ ในสถานะที่ประสบความสําเร็จ

3. สําหรับโปรไฟล์ Android หากคุณมีใบรับรองระดับกลางในห่วงโซ่ใบรับรอง ของคุณ ให้ตรวจสอบให้แน่ใจว่าได้ปรับใช้กับอุปกรณ์ Android แล้ว

    เมื่อต้องการตรวจสอบสถานะใบรับรอง ให้ไปที่**ส่วนกําหนดค่าการกําหนดค่าอุปกรณ์**  >  **Profiles**  >  **Android คุณสมบัติ CA ระดับกลาง**  >  **Properties**  >  **ใบรับรองที่เชื่อถือได้**

ถ้าคุณยังคงเห็นข้อผิดพลาดให้ตรวจสอบขั้นตอนและส่วนการแก้ไขปัญหา สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ภาพรวมสําหรับการแก้ไขปัญหาโพรไฟล์ใบรับรอง SCEP ด้วย Microsoft Intunณี](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

**ฉันปรับใช้โปรไฟล์ Wi-Fi ไปยังอุปกรณ์ Intunเป็นแสดงว่ามันประสบความสําเร็จ, แต่อุปกรณ์ไม่ได้เชื่อมต่อกับ Wi-Fi.**

สถานะสําเร็จหมายความว่า Intuna ได้ปรับใช้ส่วนกําหนดค่าเป็นการกําหนดค่าเรียบร้อยแล้ว อย่างไรก็ตาม การกําหนดค่าเหล่านี้อาจไม่ตรงกับข้อกําหนดของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายามให้ตรวจสอบบันทึกในโครงสร้างพื้นฐานและบริการการรับรองความถูกต้อง (ในตัวควบคุมจุดเข้าใช้งาน Wi-Fi และเซิร์ฟเวอร์ NPS/Radius) คุณอาจต้องทํางานร่วมกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณ หรือผู้ให้บริการ Wi-Fi บุคคลที่สาม เพื่อรวบรวมและตรวจสอบบันทึก