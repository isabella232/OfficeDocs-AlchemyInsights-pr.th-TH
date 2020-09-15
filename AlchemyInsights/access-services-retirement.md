---
title: การปลดเกษียณบริการเข้าถึง
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698701"
---
# <a name="access-services-retirement"></a>การปลดเกษียณบริการเข้าถึง

ในขณะที่เราได้ประกาศใน MC97576 ในเดือนมีนาคม๒๐๑๗และยังคงสื่อสารผ่านทางบริการการเข้าถึงปีที่ผ่านมาจะถูกถอนออกไป ขั้นตอนถัดไปในกระบวนการนี้จะเป็นการเอาออกของฐานข้อมูล Access บนเว็บที่ใช้รายการ SharePoint เป็นที่เก็บข้อมูลที่อยู่ภายใต้

**สิ่งนี้มีผลต่อฉันอย่างไร**

เริ่มต้นเดือนมิถุนายน๒๐๑๙เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint Online และปิดบริการและแอปพลิเคชันที่เหลือในเดือนเมษายน๒๐๒๐

**ฉันต้องทำอะไรบ้างเพื่อเตรียมพร้อมสำหรับการเปลี่ยนแปลงนี้**

เราขอแนะนำให้คุณสร้างแผนการเปลี่ยนสำหรับฐานข้อมูล Access บนเว็บขององค์กรของคุณ ผู้ดูแลระบบสามารถใช้ [สแกนเนอร์ของแอป SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) เพื่อขอรับสินค้าคงคลังของแอป access ที่ไซต์กำลังใช้งานอยู่

มีหลายวิธีในการโยกย้ายข้อมูลฐานข้อมูลบนเว็บของ Access:

- การนำเข้าไปยังฐานข้อมูล Access ภายในเครื่อง ( ACCDB) หรือไปยังไฟล์ Excel
- นอกจากนี้เรายังแนะนำให้สำรวจ Microsoft PowerApps เป็นแพลตฟอร์มสำหรับการสร้างโซลูชันทางธุรกิจสำหรับเว็บและอุปกรณ์เคลื่อนที่ไม่ใช่โค้ด