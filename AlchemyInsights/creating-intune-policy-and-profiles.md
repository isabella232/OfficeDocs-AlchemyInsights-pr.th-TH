---
title: สร้างนโยบายและโปรไฟล์ Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1064"
- "6700005"
ms.openlocfilehash: fac2a9e41449b4eb9b87d21d4cba4f6f5192d9c6
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715415"
---
# <a name="creating-intune-policy-and-profiles"></a>การสร้างนโยบาย Intune และโปรไฟล์

ใน Intune คุณสามารถสร้างนโยบายและโปรไฟล์ที่กระทําสิ่งที่แตกต่างกัน

- **โปรไฟล์การลงทะเบียน**: กําหนดค่าอุปกรณ์ของคุณล่วงหน้าตามแพลตฟอร์มเปิดใช้งานความเกี่ยวข้องของผู้ใช้ใช้การตรวจสอบหลายปัจจัยและอื่น ๆ

  [การลงทะเบียนอุปกรณ์คืออะไร](https://docs.microsoft.com/intune/device-enrollment)และสร้างโปรไฟล์การลงทะเบียนสําหรับ[Android](https://docs.microsoft.com/intune/android-enroll), [iOS](https://docs.microsoft.com/intune/ios-enroll), [macOS](https://docs.microsoft.com/intune/macos-enroll)และ[Windows](https://docs.microsoft.com/intune/windows-enrollment-methods)เป็นแหล่งข้อมูลที่ดี

- **นโยบายการปฏิบัติตามกฎระเบียบ**: กําหนดกฎและการตั้งค่าที่อุปกรณ์ต้องปฏิบัติตามเพื่อให้เป็นไปตามข้อกําหนด นอกจากนี้ คุณยังสามารถใช้นโยบายการปฏิบัติตามนโยบายเพื่อตรวจสอบอุปกรณ์ และแจ้งเตือนผู้ใช้ที่ไม่ปฏิบัติตามนโยบาย

  เริ่มต้นใช้งาน[นโยบายการปฏิบัติตามข้อกําหนดของอุปกรณ์](https://docs.microsoft.com/intune/device-compliance-get-started)
- **นโยบายการเข้าถึงแบบมีเงื่อนไข**: ช่วยรักษาความปลอดภัยให้กับทรัพยากรขององค์กร โดยขึ้นอยู่กับเงื่อนไขที่คุณป้อน ตัวอย่างเช่น สําหรับอุปกรณ์ที่ไม่เป็นไปตามข้อกําหนด ให้ใช้การเข้าถึงแบบมีเงื่อนไขเพื่อจํากัดการเข้าถึงอีเมลและ SharePoint

  [การเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access)[และวิธีการทั่วไปในการใช้การเข้าถึงแบบมีเงื่อนไข](https://docs.microsoft.com/intune/conditional-access-intune-common-ways-use)คือทรัพยากรที่ดีในการเริ่มต้นใช้งานคืออะไร

- **โปรไฟล์การกําหนดค่า**: จัดการคุณสมบัติและการตั้งค่าบนอุปกรณ์ รวมถึงการตั้งค่าอีเมล เพิ่มเครือข่าย WiFi ใช้เทมเพลตในตัว การควบคุมคุณสมบัติอุปกรณ์ iOS และ macOS และอื่นๆ

  เริ่มต้นใช้งาน[โปรไฟล์การกําหนดค่าอุปกรณ์](https://docs.microsoft.com/intune/device-profiles)

ลิงค์ที่เป็นประโยชน์:

- [คําถามทั่วไป ปัญหา และวิธีแก้ปัญหาด้วยนโยบายและโปรไฟล์ของอุปกรณ์ใน Intune](https://docs.microsoft.com/intune/device-profile-troubleshoot)

- [การแก้ไขปัญหานโยบายและโปรไฟล์ใน Intune](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
