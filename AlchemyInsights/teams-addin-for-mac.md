---
title: Teams Add-in for Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940694"
---
# <a name="teams-add-in-for-mac"></a>Teams Add-in for Mac

เมื่อต้องการแก้ไขปัญหาเกี่ยวกับTeams Add-in for Mac ผู้ใช้ระบบปฏิบัติการ ให้ปฏิบัติตามขั้นตอนเหล่านี้:

**ขั้นตอนที่ 1:** ถ้าคุณมีไฮบริด Exchangeภายในองค์กร (2016 CU3 หรือใหม่กว่าที่กําหนดค่า) ให้ใช้เครื่องมือ Test-HMA.ps1 เพื่อยืนยันว่า การรับรองความถูกต้องสมัยใหม่แบบไฮบริดได้รับการกําหนดค่าอย่างถูกต้อง For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).  

**หมายเหตุ** ใช้รูปแบบที่อยู่ UPN (ตัวอย่างเช่น username@contoso.com [)](mailto:username@contoso.com)ไม่ใช่ โดเมน\ชื่อผู้ใช้ วิธีนี้แม้กับผู้ใช้ที่มีExchange Onlineกล่องจดหมายของคุณ

**ขั้นตอนที่ 2:** ให้ผู้ใช้ไปที่ บัญชี  >  **เครื่องมือ**... ใน Outlook for Mac บัญชี แล้วค้นหาและเลือกบัญชี ยืนยันว่าชื่อผู้ใช้ที่แสดงรายการอยู่ในรูปแบบ UPN (ตัวอย่างเช่น [username@contoso.com](mailto:username@contoso.com))

**ขั้นตอนที่ 3:** ยืนยันว่าผู้ใช้เป็นผู้ใช้ที่มีMicrosoft Teamsสิทธิ์การใช้งาน ผู้ใช้ต้องใช้การสมัครใช้งาน Office 365 for Mac ผลิตภัณฑ์เวอร์ชัน 16.24 หรือใหม่กว่า