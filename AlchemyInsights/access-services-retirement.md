---
title: ปลดเกษียณบริการเข้าถึง
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 8886d7a6fad49e942e17f6a2f3c98542f87aae0b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495770"
---
# <a name="access-services-retirement"></a>ปลดเกษียณบริการเข้าถึง

เมื่อเราประกาศใน MC97576 ในเดือน 2017 มีนาคม และดำเนินต่อเพื่อติดต่อสื่อสารผ่านปีผ่านมาตั้งแต่แรก Access Services จะถูกถอนจาก Office 365 ขั้นต่อไปในกระบวนการนี้จะเป็นการเอาออกของฐานข้อมูลเว็บการเข้าถึงที่ใช้รายการ SharePoint เป็นการจัดเก็บข้อมูลที่อยู่ภายใต้

**วิธีไม่นี้ส่งผลต่อฉันอย่างไร**

เริ่มต้นเดือน 2019 มิถุนายน เราจะหยุดการสร้างฐานข้อมูลใหม่ของ Access ใน SharePoint แบบออนไลน์ และปิดบริการและโปรแกรมประยุกต์ใด ๆ ที่เหลือ โดย 2020 เมษายน

**สิ่งที่ฉันต้องทำเพื่อเตรียมการสำหรับการเปลี่ยนแปลงนี้หรือไม่**

เราสนับสนุนให้คุณสามารถสร้างแผนการเปลี่ยนแปลงสำหรับฐานข้อมูลเว็บการเข้าถึงขององค์กรของคุณ Admins สามารถใช้[สแกนเนอร์โปรแกรมประยุกต์ SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เมื่อต้องการรับสินค้าคงคลังของ apps Access ที่กำลังใช้ไซต์

มีหลายวิธีในการโยกย้ายข้อมูลจากฐานข้อมูล Access เว็บ:

- นำเข้าไปยังฐานข้อมูล Access ภายในเครื่อง ( ACCDB) หรือ ไปยังแฟ้ม Excel
- นอกจากนี้เรายังแนะนำสำรวจ Microsoft PowerApps เป็นแพลตฟอร์มตัวอื่นเพื่อสร้างการแก้ไขปัญหาทางธุรกิจไม่มีโค้ดสำหรับเว็บและอุปกรณ์มือถือ