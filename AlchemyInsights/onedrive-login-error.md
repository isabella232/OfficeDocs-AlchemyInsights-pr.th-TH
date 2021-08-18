---
title: OneDriveการเข้าสู่ระบบ AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112931"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDriveการเข้าสู่ระบบ AADSTS50011

ถ้าคุณได้รับข้อผิดพลาด "AADSTS50011: URL ตอบกลับที่ระบุในการร้องขอไม่ตรงกับการตอบกลับ" เมื่อลงชื่อเข้าใช้แอป OneDrive ให้ตรวจสอบรายการต่อไปนี้:

เวอร์ชันOneDriveของคุณต้องมีค่าเท่ากับหรือมากกว่าเวอร์ชัน 20.052.XXXX.XXXX เมื่อต้องการตรวจสอบเวอร์ชันของคุณ ให้คลิกที่ไอคอนOneDriveสีฟ้าในพื้นที่การแจ้งเตือน **เลือก วิธีใช้ & การตั้งค่า > การตั้งค่า >** เกี่ยวกับ

เครือข่ายของคุณอาจบล็อกการรับ **ส่งข้อมูล g.live.com** **oneclient.sfx.ms** เครือข่าย ถ้าการรับส่งข้อมูลถูกบล็อก OneDriveไม่สามารถอัปเดตตัวเองได้ ร่วมงานกับผู้ดูแลระบบเครือข่ายของคุณเพื่อให้แน่ใจว่าคุณสามารถเข้าถึง URL เหล่านั้นได้ [จุดสิ้นสุด](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)เหล่านี้ควรเข้าถึงได้กับลูกค้าที่ใช้Microsoft 365เหล่านี้

หากคุณต้องการรับเวอร์ชันปัจจุบันด้วยตนเอง OneDrive [https://aka.ms/getonedrive](https://aka.ms/getonedrive) ไปที่
