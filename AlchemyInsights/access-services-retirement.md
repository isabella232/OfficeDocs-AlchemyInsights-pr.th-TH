---
title: การเข้าถึงบริการการเกษียณอายุ
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050508"
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