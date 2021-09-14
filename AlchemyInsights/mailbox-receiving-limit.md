---
title: การบังคับใช้ขีดจํากัดของการรับกล่องจดหมาย
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316285"
---
# <a name="mailbox-receiving-limit-enforcement"></a>การบังคับใช้ขีดจํากัดของการรับกล่องจดหมาย

Microsoft เพิ่งเริ่มบังคับใช้ค่าเกณฑ์ของกล่องจดหมาย 3600 ข้อความต่อชั่วโมง ดูข้อมูลเพิ่มเติมในExchange Online[จํากัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365กล่องจดหมายที่มากกว่า 3600 ข้อความภายในหนึ่งชั่วโมงจะถูกควบคุมปริมาณเป็นเวลา 60 นาทีถัดไป 

นอกจากนี้ ขีดจํากัดคู่ผู้รับผู้ส่ง (SRP) ที่บล็อกข้อความที่ได้รับMicrosoft 365จากผู้ส่งที่ระบุจะถูกใช้งาน ถ้าผู้ส่งเดียวส่งเกิน 33% ของค่าเกณฑ์ทั้งหมดหรือข้อความ 1200 ข้อความต่อชั่วโมงที่ส่งถึงผู้รับที่ระบุ ขีดจํากัด SRP จะเริ่มต้น และกล่องจดหมายจะไม่ยอมรับข้อความจากผู้ส่งนั้นอีกต่อไป โปรดทราบว่า:

- ขีดจํากัดนี้เป็นแอปพลิเคชันของอีเมลที่ได้รับจากผู้เช่ารายอื่นๆ ภายในองค์กร หรือผู้ส่งทางอินเทอร์เน็ต
- การส่งอีเมลไปยังกล่องจดหมายจะถูกบล็อกเป็นเวลา 60 นาทีถัดไป 
- ผู้ส่งไปยังกล่องจดหมายเหล่านี้ได้รับรายงานแจ้งการไม่สามารถส่งได้ (5.2.121 หรือ 5.2.122) ที่ระบุว่ากล่องจดหมายเกินค่าเกณฑ์การส่งสูงสุดแล้ว Intra-tenant (mail within the same tenant) จะยังคงถูกส่ง
- เมื่อมีการใช้ขีดจํากัด SRP กล่องจดหมายที่รับยังคงยอมรับข้อความจากผู้ส่งอื่น

ผู้ดูแลระบบสามารถตรวจสอบกิจกรรมกล่องจดหมายปัจจุบันโดยการเข้าถึงรายงานใหม่และข้อมูลเชิงลึกในศูนย์Exchangeที่ชื่อว่า "กล่องจดหมายที่เกินขีดจํากัดการรับ" ข้อมูลเชิงลึกจะปรากฏขึ้นเฉพาะเมื่อผู้เช่ามีกล่องจดหมายที่ส่งผลกระทบต่อผู้ใช้ ในขณะที่รายงานจะปรากฏในแดชบอร์ดเสมอ แต่จะว่างเปล่า เว้นแต่ว่าผู้เช่ามีกล่องจดหมายที่ส่งผลกระทบต่อกล่องจดหมาย

For more information about insight receiving limits, see [Mailboxes exceeding receiving limits insight in the new EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

For more information about the exceeding receiving limits report, see [Mailboxes exceeding receiving limits report in the new EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report).