---
title: การแก้ไขปัญหาเหตุการณ์จากอีเมล
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658753"
---
# <a name="troubleshooting-events-from-email"></a>การแก้ไขปัญหาเหตุการณ์จากอีเมล

1. ตรวจสอบว่าฟีเจอร์ถูกเปิดใช้งานสำหรับกล่องจดหมาย:**รับ <mailbox> -EventsFromEmailConfiguration-ข้อมูลประจำตัว**

2. จากนั้นให้ดูที่ "เหตุการณ์จากอีเมล" บันทึกการ **ส่งออก-MailboxDiagnosticLogs <mailbox> -คอมโพเนนต์ TimeProfile**

3. ในบันทึก "เหตุการณ์จากอีเมล" ให้ค้นหา InternetMessageId ที่ตรงกับรายการในกล่องจดหมาย  

4. TrustScore จะกำหนดว่ารายการนั้นถูกเพิ่มหรือไม่ เหตุการณ์จะถูกเพิ่มถ้า TrustScore = "เชื่อถือได้"

TrustScore จะถูกกำหนดโดย SPF, Dkim หรือคุณสมบัติ Dmarc ซึ่งอยู่ในส่วนหัวของข้อความ

เมื่อต้องการดูคุณสมบัติเหล่านี้:

**Outlook บนเดสก์ท็อป**

- เปิดรายการ
- ไฟล์-คุณสมบัติ >-ส่วนหัวของอินเทอร์เน็ต >

หรือ

**MFCMapi**

- นำทางไปยังรายการในกล่องจดหมายเข้า
- ค้นหา PR_TRANSPORT_MESSAGE_HEADERS_W

คุณสมบัติเหล่านี้จะถูกกำหนดและบันทึกในระหว่างการขนส่งและเส้นทาง สำหรับการแก้ไขปัญหาเพิ่มเติมคุณอาจต้องติดตามการสนับสนุนการขนส่งเกี่ยวกับความล้มเหลวใน SPF, DKIM และ. หรือ DMARC