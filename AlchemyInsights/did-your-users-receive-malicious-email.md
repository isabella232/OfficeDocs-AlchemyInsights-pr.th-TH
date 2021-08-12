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
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929216"
---
# <a name="did-your-users-receive-malicious-email"></a>ผู้ใช้ของคุณได้รับอีเมลที่เป็นอันตรายหรือไม่

- ขณะนี้คุณสามารถรายงานอีเมลที่เป็นอันตรายไปยังไมโครซอฟท์โดยใช้ การส่ง[โดยผู้ดูแลระบบ ใน ศูนย์&การปฏิบัติตามข้อบังคับ](https://sip.protection.office.com/reportsubmission)

ข้อความที่ส่งในการส่ง [ของผู้ดูแลระบบ](https://sip.protection.office.com/reportsubmission) จะถูกสแกน และผลลัพธ์ต่อไปนี้แสดงอยู่ในเมนูป **ลิว** รายละเอียด

- ถ้ามีความล้มเหลวในการรับรองความถูกต้องอีเมลของผู้ส่งในเวลาที่จัดส่ง
- ข้อมูลเกี่ยวกับความนิยมของนโยบายใดๆ ที่อาจได้รับผลกระทบหรือแทนที่ผลจากข้อความ
- ผลลัพธ์การดําเนินการปัจจุบันเพื่อดูว่า URL หรือไฟล์ที่อยู่ในข้อความนั้นเป็นอันตรายหรือไม่
- ข้อเสนอแนะจากผู้ให้เกรด

ถ้าพบการแทนที่ การ rescan ควรเสร็จสมบูรณ์ในอีกหลายนาที ถ้าไม่มีปัญหาในการรับรองความถูกต้องทางอีเมลหรือถ้าการส่งอีเมลไม่ได้รับผลกระทบจากการแทนที่ การให้ข้อเสนอแนะจากผู้เกรดอาจใช้เวลาถึงหนึ่งวัน

ถ้าคุณไม่เห็นด้วยกับผลสุดท้ายในข้อความ URL หรือไฟล์ (ถูกบล็อกและไม่ถูกบล็อก) ให้ส่งข้อความอีกครั้งหลังจากผ่านไปหนึ่งวันเพื่อสแกนอีกครั้ง มีโอกาสสูงที่คะแนนจะเปลี่ยนแปลงหลังจากส่งข้อความอีกครั้ง

ขณะเดียวกัน คุณสามารถเอาอีเมลที่เป็นอันตรายออกจากกล่องขาเข้าของผู้ใช้ได้โดยการปฏิบัติตามคําแนะ [นํา](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)ในบทความนี้

- ลูกค้าที่มี Microsoft Defender Office 365สามารถ:
    - ใช้ [Threat Explorer เพื่อค้นหาและลบอีเมลที่น่าสงสัย](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [ใช้ตู้เซฟลิงก์เพื่อบล็อก](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)การเข้าถึง URL ที่เป็นอันตราย
    - ติดตามผู้ใช้ที่คลิกและเข้าถึง URL ที่เป็นอันตราย:[ดู URL ฟิชชิ่ง และคลิกข้อมูล](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)การค้นหา  &  [Get-UrlTraced](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - เริ่ม [การตรวจสอบโดยอัตโนมัติด้วยตนเอง](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

คุณยังสามารถป้องกันไฟล์และ URL ที่เป็นอันตรายได้โดยปฏิบัติตามคําแนะนําใน [การป้องกันจาก URL และไฟล์](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)ที่เป็นอันตราย