---
title: Read-Onlyข้อความการบํารุงรักษาเมื่อพยายามSharePointหรือOneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329467"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Onlyข้อความการบํารุงรักษาเมื่อพยายามSharePointหรือOneDrive

ผู้ใช้อาจได้รับข้อความ **อ่านอย่างเดียวเพื่อบํา** รุงรักษาเมื่อพยายามSharePointหรือOneDriveเหตุการณ์หนึ่งในสถานการณ์ต่อไปนี้ 

-   กิจกรรมการบํารุงรักษาที่วางแผนไว้หรือใช้งานอยู่  ตรวจสอบได้โดยนําทาง [ไปยัง ศูนย์](https://portal.office.com/adminportal/home#/messagecenter)ข้อความ
-   เหตุการณ์บริการที่มีล้ดับความร้ายแรงสูงและใช้งานอยู่ที่อาจเกิดขึ้น ตรวจสอบโปรแกรมแนะนํา/เหตุการณ์ได้โดยการนําทางไปยัง [สถานภาพ](https://portal.office.com/adminportal/home#/servicehealth)บริการ
-   สถานการณ์สมมติการกู้คืนการกู้คืนการกู้คืนการจัดการโดยอัตโนมัติรองที่อาจเกิดขึ้นเนื่องจากเหตุการณ์ที่ไม่คาดคิดบนเซิร์ฟเวอร์ซึ่งอาจอยู่นานกว่า 30 นาทีหรือนานกว่านั้น 
    
    ไม่มีศูนย์ข้อความหรือโพสต์สถานภาพบริการในการกู้คืนรองเหล่านี้ แต่คุณควรกลับมาเป็นปกติในเร็วๆ นี้

ในบางโอกาสเราสังเกตว่าหนึ่งในสามสถานการณ์ข้างต้นเป็นสาเหตุและบริการได้รับการคืนค่า แต่แคชเบราว์เซอร์ของผู้ใช้ยังไม่ถูกล้าง

โปรดพยายามล้างแคชของเบราว์เซอร์ก่อนที่จะนําทางไปยังไซต์

1. ในMicrosoft Edgeของคุณ **ให้เลือก การตั้งค่า** แล้วเลือก **ความเป็นส่วนตัว** และความปลอดภัย
2. ภายใต้ **ล้างการเรียกดู** ให้เลือก **เลือกสิ่งที่ต้องการ** ล้าง
3. เลือก **คุกกี้และข้อมูลเว็บไซต์** ที่บันทึกไว้ **แล้วเลือก** ล้าง

**หมายเหตุ**: ขั้นตอนเหล่านี้อาจแตกต่างกันเมื่อใช้เบราว์เซอร์อื่น เช่น Mozilla Firefox หรือ Google Chrome

**หมายเหตุ**: อีกตัวเลือกหนึ่งคือให้SharePointไซต์ของคุณOneDriveอยู่ในหน้าต่าง InPrivate ใหม่