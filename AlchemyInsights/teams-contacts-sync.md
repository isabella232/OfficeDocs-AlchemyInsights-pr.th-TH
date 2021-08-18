---
title: Teamsซิงค์รายชื่อผู้ติดต่อ
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
- "9004610"
- "11540"
ms.openlocfilehash: 36273e998bbf97e261dbaa49b3b57aab17216e9f0e9bd29c5d2b9f6c0d9803e4
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57900783"
---
# <a name="teams-contacts-sync"></a>Teamsซิงค์รายชื่อผู้ติดต่อ

Teamsที่ติดต่อในองค์กรของคุณ Active Directory และที่ติดต่อที่เพิ่มลงในOutlookโฟลเดอร์เริ่มต้นของผู้ใช้ ถ้าที่ติดต่อไม่แสดงMicrosoft Teams ให้ลองวิธีต่อไปนี้

**หมายเหตุ:** ถ้าข้อมูลที่ติดต่ออย่างน้อยหนึ่งรายการได้รับการอัปเดตล่าสุด อาจใช้เวลาถึง 48 ชั่วโมงเพื่อให้ที่ติดต่อซิงค์

1. ออกจากระบบTeamsและรีสตาร์ต ตรวจสอบว่าที่ติดต่อของคุณแสดงขึ้นหรือไม่
1. ล้างแคชTeams:
    1. เรียกดู **%appdata%\Microsoft\Teams**
    1. ลบเนื้อหาของโฟลเดอร์
    1. รีสตาร์ตคอมพิวเตอร์ แล้วTeamsเปิด
1. ถ้าที่ติดต่อOutlookอยู่ในรายการ ตรวจสอบให้แน่ใจว่าได้เพิ่มลงในรายการที่ติดต่อ Outlookที่ติดต่อจาก **แถบที่อยู่** ให้เลือก ไฟล์ **แล้วเลือก เพิ่มลงใน** ที่ติดต่อ
1. ตรวจสอบให้แน่ใจว่ากล่องจดหมายExchangeของผู้ใช้ถูกโฮสต์แบบออนไลน์ (ไม่ใช่ภายในองค์กร) หากต้องการข้อมูลเพิ่มเติม โปรดดู[วิธีExchange Microsoft Teams](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)โต้ตอบ
1. ตรวจสอบให้แน่ใจว่าหมายเลขโทรศัพท์ของที่ติดต่อถูกเพิ่มลงในข้อมูลที่ติดต่อแล้ว
1. ค้นหาอีเมลของที่ติดต่อในแถบค้นหา ที่ติดต่อที่คุณสามารถเรียกใช้การซิงค์ไปยังรายการที่ติดต่อได้
