---
title: วิธีการเปิดใช้งาน SSO ไม่มีรอยต่อ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 3cf751bc42322067c4b7cd9b5facb933430f2b87
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36663898"
---
# <a name="how-to-enable-seamless-sso"></a>วิธีการเปิดใช้งาน SSO ไม่มีรอยต่อ

เปิดใช้งาน SSO ที่ไม่มีรอยต่อผ่านการ[เชื่อมต่อ AD Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)
  
ถ้าคุณกำลังทำการติดตั้งใหม่ของการเชื่อมต่อ AD Azure เลือก[เส้นทางการติดตั้งแบบกำหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom) ที่หน้า**เข้าสู่ระบบของผู้ใช้**ให้เลือกตัวเลือกการ**เปิดใช้งานการเข้าสู่ระบบแบบครั้งเดียว**
  
เพื่อตรวจสอบว่าคุณได้เปิดใช้งาน SSO อย่างราบรื่นแล้ว:
  
1. เข้าสู่ระบบไปยัง[ศูนย์การจัดการไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://aad.portal.azure.com)เป็นผู้ดูแลส่วนกลาง

2. เลือก**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**ในบานหน้าต่างด้านซ้าย

3. ตรวจสอบว่า**เปิดใช้งาน**การเข้าสู่ระบบแบบครั้งเดียวอย่างราบรื่น

เมื่อต้องการเรียนรู้เพิ่มเติมโปรดดูที่[Azure ที่ใช้งานอยู่การเข้าสู่ระบบแบบครั้งเดียว: เริ่มต้นอย่างรวดเร็ว](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)
  