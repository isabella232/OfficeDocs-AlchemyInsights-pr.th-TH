---
title: ต้องการความช่วยเหลือในการจำกัดการส่งอีเมลหรือไม่
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702382"
---
# <a name="need-help-with-email-sending-limits"></a>ต้องการความช่วยเหลือในการจำกัดการส่งอีเมลหรือไม่

ด้านล่างนี้คือ **ขีดจำกัดการส่งโดยการออกแบบ** ที่บังคับใช้ในบริการ ข้อมูลเพิ่มเติมเกี่ยวกับขีดจำกัดเหล่านี้จะได้รับการบันทึกไว้[ที่นี่](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)

- เมื่อต้องการกีดกันการนำส่งข้อความจำนวนมากที่ไม่พึงประสงค์เราจะนำข้อ**จำกัดอัตราผู้รับต่อผู้ใช้ไปใช้กับข้อความขาออกและข้อความภายในทั้งหมด** ใน Sku ทั้งหมดขีดจำกัดนี้คือ**ผู้รับ๑๐,๐๐๐ต่อวัน**  ลูกค้าที่จำเป็นต้องส่งอีเมลการค้าจำนวนมากที่ถูกต้องตามกฎหมาย (ตัวอย่างเช่นจดหมายข่าวของลูกค้า) ควรใช้ผู้ให้บริการของบริษัทอื่นที่มีความเชี่ยวชาญในบริการเหล่านี้
    - **หมายเหตุ**: เมื่อถึงขีดจำกัดอัตราผู้รับข้อความจะไม่สามารถส่งจากกล่องจดหมายได้จนกว่าจำนวนผู้รับที่ส่งข้อความในช่วง24ชั่วโมงที่ผ่านมาจะลดลงต่ำกว่าขีดจำกัด ผู้ใช้จะไม่สามารถส่งข้อความได้จนกว่าจุดนั้น
- ขีดจำกัดอัตราข้อความ **30 ข้อความต่อนาที** จะถูกนำไปใช้ใน sku ทั้งหมด สิ่งนี้จะกำหนดจำนวนข้อความที่ผู้ใช้สามารถส่งจากบัญชีผู้ใช้ Exchange Online ของพวกเขาภายในช่วงเวลาที่ระบุได้
- **จำนวนสูงสุดของผู้รับที่ได้รับอนุญาตในเขตข้อมูลถึง, สำเนาถึงและสำเนาลับ**ถึงสำหรับข้อความอีเมลเดียวทั้งหมดจะเป็น**ผู้รับ๑๐๐๐** เมื่อต้องการกำหนดขีดจำกัดนี้เองให้ไป[ที่นี่](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)
