---
title: โปรไฟล์ของ Intune สำหรับ wi-fi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696280"
---
# <a name="intune-wi-fi-profiles"></a>โปรไฟล์ของ Intune สำหรับ wi-fi

การดำเนินการการเชื่อมต่อ Wi-fi ที่ประสบความสำเร็จสำหรับไคลเอ็นต์ MDM จะขึ้นอยู่กับโปรไฟล์ที่มีการปรับใช้อย่างถูกต้องซึ่งแสดงถึงความต้องการของโครงสร้างพื้นฐาน Wi-fi ขององค์กร เมื่อต้องการตรวจสอบการตั้งค่าที่เหมาะสมสำหรับแพลตฟอร์มไคลเอ็นต์ที่คุณกำลังตรวจสอบให้ดูที่: 

[เพิ่มการตั้งค่า Wi-fi สำหรับอุปกรณ์ที่ใช้ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[เพิ่มการตั้งค่า Wi-fi สำหรับอุปกรณ์ Android ที่เฉพาะเจาะจงและมีการจัดการทั้งหมดใน Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[เพิ่มการตั้งค่า Wi-fi สำหรับอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[เพิ่มการตั้งค่า Wi-fi สำหรับ Windows 10 และอุปกรณ์รุ่นที่ใหม่กว่าใน Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[นำเข้าการตั้งค่า wi-fi สำหรับอุปกรณ์ Windows ใน Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**ปัญหาทั่วไป**

**ฉันกำลังปรับใช้โปรไฟล์ Wi-fi ที่ขึ้นอยู่กับใบรับรองที่มีการปรับใช้ที่ระบุไว้ในโปรไฟล์ Wi-Fi อย่างไรก็ตามโปรไฟล์การกำหนดค่าจะแสดงสถานะข้อผิดพลาด**

ตรวจสอบว่าอุปกรณ์ของคุณได้รับใบรับรองแล้วหรือไม่

1. ใน Intune ให้ไปที่**อุปกรณ์ทั้งหมด**แล้วเลือกอุปกรณ์ >**การกำหนดค่าอุปกรณ์**

2. ตรวจสอบว่าโปรไฟล์ที่คาดไว้ทั้งหมดอยู่ในรายการและสถานะที่เสร็จสมบูรณ์แล้ว

3. สำหรับโปรไฟล์ Android ถ้าคุณมีใบรับรองระดับกลางในสายใบรับรองของคุณให้ตรวจสอบให้แน่ใจว่าพวกเขาได้รับการปรับใช้กับอุปกรณ์ Android

    เมื่อต้องการตรวจสอบสถานะใบรับรองให้ไปที่โปรไฟล์**การกำหนดค่าอุปกรณ์**  >  **Profiles**  >  **Android คุณสมบัติ CA กลาง**  >  **Properties**  >  ที่**เชื่อถือได้ใบรับรองที่เชื่อถือ**ได้

ถ้าคุณยังคงเห็นข้อผิดพลาดให้ตรวจทานขั้นตอนและการแก้ไขปัญหาส่วน สำหรับข้อมูลเพิ่มเติมให้ดูที่[ภาพรวมสำหรับการแก้ไขปัญหาส่วนกำหนดค่า SCEP ที่มี Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

**ฉันจัดวางโปรไฟล์ Wi-fi ไปยังอุปกรณ์ Intune จะแสดงว่าเสร็จเรียบร้อยแล้วแต่อุปกรณ์ไม่ได้เชื่อมต่อกับ Wi-fi**

สถานะที่เสร็จสมบูรณ์หมายความว่า Intune ได้ปรับใช้โปรไฟล์ตามที่ได้รับการกำหนดค่าเรียบร้อยแล้ว อย่างไรก็ตามการกำหนดค่าเหล่านี้อาจไม่ตรงกับความต้องการของเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับการเชื่อมต่อที่พยายามตรวจสอบบันทึกในบริการโครงสร้างพื้นฐานและการรับรองความถูกต้อง (บนเซิร์ฟเวอร์ตัวควบคุมจุดเข้าใช้งาน Wi-fi และ NPS/Radius) คุณอาจต้องทำงานกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณหรือผู้จำหน่าย wi-fi ของบริษัทอื่นเพื่อรวบรวมและตรวจทานบันทึก