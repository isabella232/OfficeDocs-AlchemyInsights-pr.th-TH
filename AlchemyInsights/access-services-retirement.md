---
title: การเข้าถึงบริการการเกษียณอายุ
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/18/2019
ms.locfileid: "36747805"
---
# <a name="access-services-retirement"></a>การเข้าถึงบริการการเกษียณอายุ

ในขณะที่เราได้ประกาศใน MC97576 มีนาคม๒๐๑๗และยังคงสื่อสารในปีที่ผ่านมาบริการการเข้าถึงจะถูกตัดออกจาก Office ๓๖๕ ขั้นตอนต่อไปในกระบวนการนี้จะเป็นการเอาออกของฐานข้อมูลการเข้าถึงเว็บที่ใช้รายการ SharePoint เป็นการจัดเก็บข้อมูลพื้นฐานของพวกเขา

**วิธีนี้ส่งผลต่อฉันอย่างไร**

เริ่มตั้งแต่เดือนมิถุนายน๒๐๑๙เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint แบบออนไลน์และปิดบริการและแอปที่เหลืออยู่โดย๒๐๒๐เดือนเมษายน

**ฉันต้องทำอะไรเพื่อเตรียมความพร้อมสำหรับการเปลี่ยนแปลงนี้**

เราขอแนะนำให้คุณสร้างแผนการเปลี่ยนแปลงสำหรับฐานข้อมูลเว็บขององค์กรของคุณ ผู้ดูแลระบบสามารถใช้[สแกนเนอร์แอพลิเคชัน SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เพื่อขอรับสินค้าคงคลังของโปรแกรมประยุกต์ access ที่ไซต์กำลังใช้อยู่

มีหลายวิธีในการโยกย้ายข้อมูลในฐานข้อมูลเว็บของ Access:

- การนำเข้าไปยังฐานข้อมูล Access ภายในเครื่อง ( ACCDB) หรือไปที่ไฟล์ Excel
- นอกจากนี้เรายังแนะนำให้คุณสำรวจ Microsoft PowerApps เป็นแพลตฟอร์มอื่นเพื่อสร้างโซลูชันทางธุรกิจแบบไม่มีรหัสสำหรับเว็บและอุปกรณ์เคลื่อนที่