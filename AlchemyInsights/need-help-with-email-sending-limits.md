---
title: ต้องการความช่วยเหลือเกี่ยวกับขีดจํากัดการส่งอีเมลหรือไม่
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b55654f56ab405c93934fd1a0917f50c053b09466e877e1255adbd28db83d93f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097535"
---
# <a name="need-help-with-email-sending-limits"></a>ต้องการความช่วยเหลือเกี่ยวกับขีดจํากัดการส่งอีเมลหรือไม่

ด้านล่างนี้คือ **ขีดจํากัดการส่งตาม** การออกแบบที่ถูกบังคับใช้ในบริการ ข้อมูลเพิ่มเติมเกี่ยวกับขีดจํากัดเหล่านี้ได้บันทึก[ที่นี่](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)

- ในการลบการส่งข้อความเป็นกลุ่มที่ไม่พึงประสงค์ เราจะใช้ขีดจํากัดอัตราของผู้รับต่อ **ผู้ใช้กับข้อความขาออกและข้อความ** ภายในทั้งหมด ใน SKU ทั้งหมด ขีดจํากัดคือ **10,000 คน** ต่อวัน  ลูกค้าที่ต้องการส่งอีเมลเชิงพาณิชย์เป็นกลุ่มที่ถูกต้องตามกฎหมาย (ตัวอย่างเช่น จดหมายข่าวลูกค้า) ควรใช้ผู้ให้บริการของบริษัทอื่นที่ขายดีในบริการเหล่านี้
    - **หมายเหตุ**: เมื่อถึงขีดจํากัดอัตราของผู้รับข้อความแล้ว ไม่สามารถส่งข้อความจากกล่องจดหมายได้จนกว่าจะถึงจํานวนผู้รับที่ส่งข้อความในช่วง 24 ชั่วโมงที่ผ่านมาลดขีดจํากัด ผู้ใช้จะไม่สามารถส่งข้อความได้จนกว่าจะถึงจุดนั้น
- ขีดจํากัดอัตราข้อความ **30 ข้อความต่อ** นาทีจะถูกปรับใช้ใน SKU ทั้งหมด วิธีนี้จะระบุปริมาณข้อความที่ผู้ใช้สามารถส่งจากExchange Onlineของข้อความภายในช่วงเวลาที่ระบุ
- จํานวน **ผู้รับสูงสุดที่อนุญาตใน** เขตข้อมูล ถึงส.ค. และ ส. ของข้อความอีเมลเดียว ใน SKU ทั้งหมด คือ **1000** ผู้รับ เมื่อต้องการปรับแต่งขีดจํากัดนี้ [ให้ไปที่](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)นี่
