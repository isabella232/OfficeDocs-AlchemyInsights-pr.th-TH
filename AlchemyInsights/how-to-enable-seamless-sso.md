---
title: วิธีการเปิดใช้งาน SSO แบบไร้รอยต่อ
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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "36663898"
---
# <a name="how-to-enable-seamless-sso"></a>วิธีการเปิดใช้งาน SSO แบบไร้รอยต่อ

เปิดใช้งาน SSO ที่ราบรื่นผ่าน[การเชื่อมต่อโฆษณา Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)
  
ถ้าคุณกําลังทําการติดตั้งใหม่ของ Azure AD Connect ให้เลือก[เส้นทางการติดตั้งแบบกําหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom) ที่หน้า**ลงชื่อเข้าใช้ของผู้ใช้**ให้เลือกตัวเลือก**เปิดใช้งานการลงชื่อเข้าใช้ครั้งเดียว**
  
เมื่อต้องการตรวจสอบว่า คุณได้เปิดใช้งาน SSO แบบไม่มีรอยต่ออย่างถูกต้อง:
  
1. เข้าสู่ระบบไปยัง[ศูนย์การจัดการ Azure Active Directory](https://aad.portal.azure.com)เป็นผู้ดูแลระบบส่วนกลาง

2. เลือก**ไดเรกทอรีที่ใช้งานอยู่ของ Azure**ในบานหน้าต่างด้านซ้าย

3. ตรวจสอบว่าการลงชื่อเข้าระบบครั้งเดียวแบบไม่มีรอยต่อ**ถูกเปิดใช้งาน**

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดูที่[Azure Active Directory แบบครั้งเดียวที่ราบรื่น: เริ่มต้นใช้งานด่วน](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)
  