---
title: การแก้ไขปัญหากิจกรรมจากอีเมล
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834858"
---
# <a name="troubleshooting-events-from-email"></a>การแก้ไขปัญหากิจกรรมจากอีเมล

1. ตรวจสอบว่ามีการเปิดใช้งานฟีเจอร์นี้กับกล่องจดหมายหรือไม่ **: Get-EventsFromAmailConfiguration <mailbox> -Identity**

2. จากนั้นดูที่บันทึก 'เหตุการณ์จากอีเมล' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. ในบันทึก 'กิจกรรมจากอีเมล' ให้ค้นหา InternetMessageId ที่ตรงกับรายการในกล่องจดหมาย  

4. TrustScore จะระบุว่ารายการถูกเพิ่มหรือไม่ เหตุการณ์จะถูกเพิ่มถ้า TrustScore = "Trusted" เท่านั้น

TrustScore จะถูกกําหนดโดยคุณสมบัติ SPF, Dkim หรือ Dmarc ซึ่งอยู่ในส่วนหัวของข้อความ

เมื่อต้องการดูคุณสมบัติเหล่านี้:

**Outlook บนเดสก์ท็อป**

- เปิดรายการ
- File -> Properties ->ส่วนหัวอินเทอร์เน็ต

หรือ

**MFCMapi**

- นําทางไปยังรายการในกล่องจดหมายเข้า
- ค้นหาPR_TRANSPORT_MESSAGE_HEADERS_W

คุณสมบัติเหล่านี้จะถูกกําหนดและบันทึกระหว่างการส่งผ่านและการกําหนดเส้นทาง For further troubleshooting, you may need to follow up with Transport Support about the failures in SPF, DKIM and.or DMARC.