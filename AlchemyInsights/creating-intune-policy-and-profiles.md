---
title: สร้างนโยบายของ Intune และโปรไฟล์ของ Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: 9026beac824ebc3849241dbb534c27b00ef1d0eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47746778"
---
# <a name="creating-intune-policy-and-profiles"></a>การสร้างนโยบายและโพรไฟล์ของ Intune

ใน Intune คุณสามารถสร้างนโยบายและโปรไฟล์ที่ทำสิ่งต่างๆได้

- **โปรไฟล์การลงทะเบียน**: กำหนดการอุปกรณ์ของคุณตาม platform ให้เปิดใช้งานความสัมพันธ์ของผู้ใช้ใช้การรับรองความถูกต้องแบบหลายปัจจัยและอื่นๆ

  การ[ลงทะเบียนอุปกรณ์คืออะไร](https://docs.microsoft.com/intune/device-enrollment)และสร้างโปรไฟล์การลงทะเบียนสำหรับ[Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)และ[Windows](https://docs.microsoft.com/intune/windows-enrollment-methods)เป็นแหล่งข้อมูลที่ดี

- **นโยบายการปฏิบัติตามกฎระเบียบ**: กำหนดกฎและการตั้งค่าที่อุปกรณ์ต้องเป็นไปตามเพื่อให้สอดคล้องกัน นอกจากนี้คุณยังสามารถใช้นโยบายการปฏิบัติตามนโยบายเพื่อตรวจสอบอุปกรณ์และแจ้งให้ผู้ใช้ที่ไม่ปฏิบัติตามข้อบังคับ

  เริ่มต้นใช้งาน[นโยบายการปฏิบัติตามนโยบายของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)
- **นโยบายการเข้าถึงตามเงื่อนไข**: ช่วยรักษาความปลอดภัยทรัพยากรขององค์กรทั้งนี้ขึ้นอยู่กับเงื่อนไขที่คุณใส่ ตัวอย่างเช่นสำหรับอุปกรณ์ที่ไม่สอดคล้องกันให้ใช้การเข้าถึงตามเงื่อนไขเพื่อจำกัดการเข้าถึงอีเมลและ SharePoint

  การ[เข้าถึงเงื่อนไข](https://docs.microsoft.com/intune/conditional-access)และ[วิธีทั่วไปในการใช้การเข้าถึง](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)แบบมีเงื่อนไขคือทรัพยากรที่ดีในการเริ่มต้นใช้งาน

- **โปรไฟล์การกำหนดค่า**: จัดการฟีเจอร์และการตั้งค่าบนอุปกรณ์รวมถึงการตั้งค่าอีเมลเพิ่มเครือข่าย WiFi ใช้เทมเพลตที่มีอยู่แล้วภายในตัวควบคุมอุปกรณ์ IOS และ macOS และอื่นๆ

  เริ่มต้นใช้งานที่[โปรไฟล์การกำหนดค่าอุปกรณ์](https://docs.microsoft.com/intune/device-profiles)

ลิงก์ที่มีประโยชน์:

- [คำถามทั่วไปปัญหาและวิธีแก้ไขปัญหาเกี่ยวกับนโยบายของอุปกรณ์และโปรไฟล์ใน Intune](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [การแก้ไขปัญหานโยบายและโปรไฟล์ใน Intune](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
