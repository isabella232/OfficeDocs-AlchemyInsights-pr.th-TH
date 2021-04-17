---
title: วิธีการเปิดใช้งาน SSO อย่างราบรื่น
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825750"
---
# <a name="how-to-enable-seamless-sso"></a>วิธีการเปิดใช้งาน SSO อย่างราบรื่น

เปิดใช้งาน SSO อย่างราบรื่น[ผ่าน Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)
  
ถ้าคุณติดตั้ง Azure AD Connect ใหม่ ให้เลือกเส้นทางการติดตั้ง [แบบปรับแต่ง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)เอง ที่ **หน้าลงชื่อเข้าใช้ของผู้ใช้** ให้เลือกตัวเลือก **เปิดใช้งานการเข้าสู่ระบบโดย** ลงชื่อเข้าใช้ครั้งเดียว
  
เมื่อต้องการตรวจสอบว่าคุณได้เปิดใช้งาน SSO อย่างราบรื่นอย่างถูกต้อง:
  
1. ลงชื่อเข้าใช้ศูนย์การจัดการ [Azure Active Directory](https://aad.portal.azure.com) ในฐานะผู้ดูแลระบบส่วนกลาง

2. เลือก **Azure Active Directory** ในบานหน้าต่างด้านซ้าย

3. ตรวจสอบว่า เปิดใช้งานการเข้าสู่ระบบโดย **ลงชื่อเข้าใช้ครั้งเดียวอย่าง** ราบรื่น

เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู [การลงชื่อเข้าระบบครั้งเดียวอย่าง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)ราบรื่นของ Azure Active Directory: เริ่มต้นใช้งานด่วน
  