---
title: เกี่ยวกับการอัปเดตความปลอดภัยของ Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482985"
---
# <a name="about-exchange-server-security-updates"></a>เกี่ยวกับการอัปเดตความปลอดภัยของ Exchange Server

Microsoft ได้เผยแพร่ชุดการอัปเดตความปลอดภัยที่วิกฤติใน Exchange Server ภายในองค์กร เวอร์ชันของเซิร์ฟเวอร์ที่ได้รับผลกระทบคือระดับการอัปเดตใดๆ ของ Exchange Server 2010, 2013, 2016 และ 2019 Exchange Online จะไม่ได้รับผลกระทบ แต่ถ้าคุณมีเซิร์ฟเวอร์ Exchange ภายในองค์กรบางส่วนเนื่องจากการกําหนดค่าแบบไฮบริด เซิร์ฟเวอร์เหล่านั้นอาจมีความเสี่ยง

เมื่อต้องการอัปเดตเซิร์ฟเวอร์ภายในองค์กรของคุณจะต้องใช้งาน Exchange เวอร์ชันต่อไปนี้เป็นอย่างน้อย:

- Exchange 2010 Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 CU 19 หรือ CU 18
- Exchange Server 2019 CU 8 หรือ CU 7

โปรดดูประกาศต่อไปนี้เกี่ยวกับสถานที่ตั้งของการแก้ไข: [เผยแพร่แล้ว: การอัปเดตความปลอดภัยของ Exchange Server ในเดือนมีนาคม 2021](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**หมายเหตุสําคัญ:**

การติดตั้งการอัปเดตจะใช้งานไม่ได้ถ้าเซิร์ฟเวอร์ภายในองค์กรของคุณไม่ได้ใช้ Exchange เวอร์ชันที่ต้องใช้ ตามรายการข้างต้น

ถ้าติดตั้งการอัปเดตด้วยตนเอง โปรดอ่านส่วน "ปัญหาที่ทราบแล้ว" ของการอัปเดตบทความ KB เพื่อดูข้อมูลสําคัญ การอัปเดตการรักษาความปลอดภัยต้องเรียกใช้จากพร้อมท์ CMD/PowerShell ด้วยสิทธิ์ผู้ดูแล!
