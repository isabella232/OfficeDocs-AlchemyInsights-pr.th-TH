---
title: ปลดเกษียณบริการเข้าถึง
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769483"
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