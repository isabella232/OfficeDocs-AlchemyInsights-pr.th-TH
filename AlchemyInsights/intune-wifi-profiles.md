---
title: โปรไฟล์Wi-Fi Intun
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
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028249"
---
# <a name="intune-wi-fi-profiles"></a>โปรไฟล์Wi-Fi Intun

การปรับใช้การเชื่อมต่อWi-Fiของ MDM ที่ประสบความสําเร็จขึ้นอยู่กับโปรไฟล์ที่ปรับใช้ได้อย่างถูกต้อง ซึ่งสะท้อนถึงความต้องการของWi-Fiโครงสร้างพื้นฐานขององค์กร เมื่อต้องการตรวจสอบการตั้งค่าที่เหมาะสมของแพลตฟอร์มไคลเอ็นต์ที่คุณตรวจสอบ ให้ดู: 

[เพิ่มWi-Fiอุปกรณ์ที่ใช้ Android ใน Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[เพิ่มWi-Fiการตั้งค่าเฉพาะของ Android Enterprise ที่มีการจัดการอย่างเต็มรูปแบบMicrosoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[เพิ่มWi-Fiอุปกรณ์ iOS และ iPadOS ใน Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[เพิ่มWi-Fiการตั้งค่าของคุณWindows 10และอุปกรณ์ที่ใหม่กว่าใน Intuned](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[นําเข้าWi-Fiการตั้งค่าการนําWindowsอุปกรณ์ใน Intuned](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**ปัญหาทั่วไป**

**ฉันปรับใช้โปรไฟล์Wi-Fiที่ขึ้นอยู่กับใบรับรองที่ปรับใช้ที่ระบุไว้ในWi-Fiโปรไฟล์ของคุณ อย่างไรก็ตาม โปรไฟล์การกําหนดค่าจะแสดงสถานะข้อผิดพลาด**

ตรวจสอบว่าอุปกรณ์ของคุณได้รับใบรับรองแล้ว

1. ใน Intuned ให้ไปที่ **อุปกรณ์ทั้งหมด** แล้วเลือกอุปกรณ์> **การกําหนดค่า** อุปกรณ์

2. ตรวจสอบว่าโปรไฟล์ที่คาดไว้ทั้งหมดอยู่ในรายการและอยู่ในสถานะประสบความสเร็จ

3. For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.

    เมื่อต้องการตรวจสอบสถานะใบรับรอง ให้ไปที่ โปรไฟล์การ **กําหนดค่า**  >  **อุปกรณ์**  >  **คุณสมบัติ CA**  >  **ระดับกลางของ** Android  >  **ใบรับรองที่เชื่อถือได้**

ถ้าคุณยังคงเห็นข้อผิดพลาด อยู่ ให้ตรวจทานขั้นตอนและส่วนการแก้ไขปัญหา For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**ฉันปรับใช้Wi-Fiโปรไฟล์กับอุปกรณ์ Intun1 แสดงว่าประสบความสเร็จ แต่อุปกรณ์ไม่ได้เชื่อมต่อกับ Wi-Fi**

สถานะประสบความสเร็จหมายความว่า Intuned ได้ปรับใช้โปรไฟล์ตามที่กําหนดค่าแล้ว อย่างไรก็ตาม การกําหนดค่าเหล่านี้อาจไม่ตรงกับข้อกําหนดเครือข่ายและ/หรือการรับรองความถูกต้องของคุณ For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server). คุณอาจต้องร่วมงานกับทีมโครงสร้างพื้นฐานเครือข่ายของคุณ หรือผู้จัดWi-Fiอื่น เพื่อรวบรวมและตรวจทานบันทึก