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
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687277"
---
# <a name="access-services-retirement"></a>การเข้าถึงบริการการเกษียณอายุ

ในเดือนมีนาคม 2017 และยังคงสื่อสารกันอย่างต่อเนื่องตลอดปีที่ผ่านมา ขั้นตอนถัดไปในกระบวนการนี้จะเป็นการเอาฐานข้อมูล Access Web ที่ใช้รายการ SharePoint เป็นที่เก็บข้อมูลต้นแบบออก

**สิ่งนี้ส่งผลต่อฉันอย่างไร**

เริ่ม 2019 มิถุนายน เราจะหยุดการสร้างฐานข้อมูล Access ใหม่ใน SharePoint Online และปิดบริการและแอปที่เหลือภายในเดือนเมษายน 2020

**ฉันต้องทําอะไรบ้างเพื่อเตรียมการเปลี่ยนแปลงนี้**

เราสนับสนุนให้คุณสร้างแผนการเปลี่ยนสําหรับฐานข้อมูลเว็บ Access ขององค์กรของคุณ ผู้ดูแลระบบสามารถใช้[โปรแกรมสแกนโปรแกรมประยุกต์ SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)เพื่อขอรับสินค้าคงคลังของโปรแกรมประยุกต์ Access ที่ไซต์กําลังใช้อยู่

มีหลายวิธีในการย้ายข้อมูลฐานข้อมูลเว็บ Access:

- การนําเข้าฐานข้อมูล Access ภายในเครื่อง (.AS) ACCDB) หรือไปยังไฟล์ Excel
- เราขอแนะนําให้สํารวจ Microsoft PowerApps เป็นแพลตฟอร์มอื่นเพื่อสร้างโซลูชันทางธุรกิจที่ไม่มีรหัสสําหรับเว็บและโทรศัพท์มือถือ