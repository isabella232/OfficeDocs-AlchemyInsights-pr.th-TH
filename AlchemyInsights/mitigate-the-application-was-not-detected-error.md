---
title: ลดข้อผิดพลาด แอปพลิเคชันไม่พบข้อผิดพลาด
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026133"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>แก้ไขข้อผิดพลาด "ไม่พบแอปพลิเคชัน"

ข้อผิดพลาดการติดตั้งแอป "ไม่พบแอปพลิเคชันหลังจากการติดตั้งเสร็จสมบูรณ์" ที่รายงานโดย Intun1 อาจเกิดขึ้นบนแพลตฟอร์ม OS หลักทั้งหมด (Windows, iOS และ Android)

สถานการณ์ทั่วไปที่สร้างข้อผิดพลาดนี้ ได้แก่

- แอปได้รับการอัปเดตภายนอก Intun1 (จากร้านค้าแอปของบริษัทอื่น) หลังจากการปรับใช้ครั้งแรก ตัวอย่างเช่น บางแอปพลิเคชัน เช่น Google Chrome อาจอัปเดตโดยอัตโนมัติ
- ผู้ใช้ถอนการติดตั้งแอปหลังจากการติดตั้งครั้งแรก

เมื่อต้องการลดปัญหานี้ ก่อนอื่นให้ตรวจสอบอุปกรณ์ที่ได้รับผลกระทบเพื่อระบุสถานการณ์ที่ข้อผิดพลาดเกิดขึ้น

- ถ้าแอปได้รับการอัปเดตภายนอก Intun1 สามารถตั้งค่าการปรับใช้แอปให้ละเว้นเวอร์ชันของแอปพลิเคชันได้ To do so, under **App Configuration > App Information**, set Ignore **App** version to **Yes**.
- เมื่อ targeting the client, it may be appropriate to deploy the application as "required," and to ensure that the latest version is deployed.
- หรือ บนแพลตฟอร์ม iOS คุณสามารถใช้ฟังก์ชัน **autoupdate** ที่เกี่ยวข้องกับโปรแกรมการซื้อของ Apple ซึ่งสามารถกําหนดค่าให้อัปเดตเป็นแอปพลิเคชันเวอร์ชันใหม่โดยอัตโนมัติเมื่อพร้อมใช้งาน

For more information about troubleshooting app installation issues, please see [Troubleshoot app installation](https://docs.microsoft.com/intune/troubleshoot-app-install)issues .
