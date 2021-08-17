---
title: ผู้ใช้ของคุณได้รับอีเมลที่เป็นอันตราย
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 608e2226c055f58ecf4f62e3c913106a6d319190ed6b317508e41514c12ba5d0
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893422"
---
# <a name="did-your-users-receive-malicious-email"></a>ผู้ใช้ของคุณได้รับอีเมลที่เป็นอันตรายหรือไม่

ขณะนี้คุณสามารถรายงานอีเมลที่เป็นอันตรายไปยัง Microsoft[โดยใช้ การส่ง Microsoft 365 Defenderพอร์ทัล](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

ข้อความที่ส่งมาใน [การส่งของผู้ดูแลระบบ](https://security.microsoft.com/reportsubmission?viewid=admin) จะถูกสแกน และผลลัพธ์ต่อไปนี้จะแสดงในเมนูปลิวรายละเอียด

- ถ้ามีความล้มเหลวในการรับรองความถูกต้องอีเมลของผู้ส่งในเวลาที่จัดส่ง
- ข้อมูลเกี่ยวกับความที่ตรงกับนโยบายใดๆ ที่อาจได้รับผลกระทบหรือแทนที่ข้อขัดแย้งของข้อความ
- ผลลัพธ์การดําเนินการปัจจุบันเพื่อดูว่า URL หรือไฟล์ที่อยู่ในข้อความนั้นเป็นอันตรายหรือไม่
- ข้อเสนอแนะจากผู้ให้เกรด

ถ้าพบการแทนที่ การ rescan ควรเสร็จสมบูรณ์ในอีกหลายนาที ถ้าไม่มีปัญหาในการรับรองความถูกต้องทางอีเมลหรือถ้าการส่งไม่ได้รับผลกระทบจากการแทนที่ การให้ข้อเสนอแนะจากผู้เกรดอาจใช้เวลาถึงหนึ่งวัน

หากคุณไม่เห็นด้วยกับผลสุดท้ายในข้อความ URL หรือไฟล์ (ถูกบล็อกและไม่ถูกบล็อก) ให้ส่งข้อความอีกครั้งหลังจากผ่านไปหนึ่งวันเพื่อสแกนอีกครั้ง มีโอกาสสูงที่คะแนนจะเปลี่ยนแปลงหลังจากส่งข้อความอีกครั้ง

ขณะเดียวกัน คุณสามารถเอาอีเมลที่เป็นอันตรายออกจากกล่องขาเข้าของผู้ใช้ได้โดยการปฏิบัติตามคําแนะ [นํา](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)ในบทความนี้

- ลูกค้าที่มี Microsoft Defender Office 365สามารถ:
  - ใช้ [Threat Explorer เพื่อค้นหาและลบอีเมลที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [ใช้ตู้เซฟลิงก์เพื่อบล็อก](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links)การเข้าถึง URL ที่เป็นอันตราย
  - ติดตามผู้ใช้ที่คลิกและเข้าถึง URL ที่เป็นอันตราย:[ดู URL ฟิชชิ่งและคลิกข้อมูล](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)การค้นหา  &  [Get-UrlTraced](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - เริ่ม [การตรวจสอบอัตโนมัติด้วยตนเอง](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

คุณยังสามารถป้องกันไฟล์และ URL ที่เป็นอันตรายได้โดยปฏิบัติตามคําแนะนําใน [การป้องกันจาก URL และไฟล์](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)ที่เป็นอันตราย
