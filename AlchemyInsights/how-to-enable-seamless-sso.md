---
title: วิธีเปิดใช้งาน SSO อย่างราบรื่น
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780546"
---
# <a name="how-to-enable-seamless-sso"></a>วิธีเปิดใช้งาน SSO อย่างราบรื่น

เปิดใช้งาน SSO อย่างราบรื่นผ่าน[AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)
  
ถ้าคุณกำลังทำการติดตั้งใหม่ของ Azure AD Connect ให้เลือก[เส้นทางการติดตั้งแบบกำหนดเอง](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom) ที่หน้า**ลงชื่อเข้าใช้ของผู้ใช้**ให้เลือกตัวเลือก**เปิดใช้งานการลงชื่อเข้าใช้ครั้งเดียว**
  
เมื่อต้องการตรวจสอบว่าคุณได้เปิดใช้งานอย่างราบรื่น SSO อย่างถูกต้อง:
  
1. ลงชื่อเข้าใช้ [ศูนย์การจัดการไดเรกทอรีของ Azure ที่ใช้งานอยู่](https://aad.portal.azure.com) ในฐานะผู้ดูแลระบบส่วนกลาง

2. เลือก **Azure Active directory** ในบานหน้าต่างด้านซ้าย

3. ตรวจสอบว่า **เปิดใช้งาน**การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น

เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่[ไดเรกทอรีที่ใช้งานอยู่ของ Azure การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น: เริ่มต้น](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)
  