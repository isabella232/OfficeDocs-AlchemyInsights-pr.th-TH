---
title: ข้อผิดพลาดการเข้าสู่ระบบ OneDrive AADSTS50011
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
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982548"
---
# <a name="onedrive-login-error-aadsts50011"></a>ข้อผิดพลาดการเข้าสู่ระบบ OneDrive AADSTS50011

ถ้าคุณได้รับข้อผิดพลาด "AADSTS50011: URL ตอบกลับที่ระบุในการร้องขอไม่ตรงกับการตอบกลับ" เมื่อลงชื่อเข้าใช้แอป OneDrive ให้ตรวจสอบดังต่อไปนี้:

เวอร์ชัน OneDrive ของคุณจำเป็นต้องมีค่าเท่ากับหรือมากกว่าเวอร์ชัน 20.052. XXXX XXXX . เมื่อต้องการตรวจสอบเวอร์ชันของคุณให้คลิกที่ไอคอน OneDrive สีน้ำเงินในพื้นที่การแจ้งเตือนเลือก **วิธีใช้ & การตั้งค่า > การตั้งค่า > เกี่ยวกับ**

เครือข่ายของคุณอาจบล็อกการรับส่งข้อมูลไปยัง **g.live.com** และ **oneclient.sfx.ms** ถ้าการรับส่งข้อมูลดังกล่าวถูกบล็อก OneDrive จะไม่สามารถอัปเดตได้เองได้ ทำงานกับผู้ดูแลระบบเครือข่ายของคุณเพื่อให้แน่ใจว่าคุณสามารถเข้าถึง Url เหล่านั้นได้ จุดสิ้นสุด[เหล่านี้](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)ควรสามารถเข้าถึงได้สำหรับลูกค้าที่ใช้แผน Microsoft ๓๖๕

ถ้าคุณต้องการรับเวอร์ชันปัจจุบันของ OneDrive [https://aka.ms/getonedrive](https://aka.ms/getonedrive) ให้เยี่ยมชมด้วยตนเอง
