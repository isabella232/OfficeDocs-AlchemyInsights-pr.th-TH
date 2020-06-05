---
title: การแก้ไขปัญหาเหตุการณ์จากอีเมล
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569401"
---
# <a name="troubleshooting-events-from-email"></a>การแก้ไขปัญหาเหตุการณ์จากอีเมล

1. ตรวจสอบลักษณะการทํางานถูกเปิดใช้งานสําหรับกล่องจดหมาย:**รับเหตุการณ์From-อีเมลการกําหนดค่า-รหัสประจําตัว <mailbox> **

2. แล้วดูที่ 'เหตุการณ์จากอีเมล' บันทึก**การส่งออก MailboxDiagnosticLogs <mailbox> -เวลาคอมโพเนนต์Profile**

3. ในบันทึก 'เหตุการณ์จากอีเมล' ให้ค้นหา InternetMessageId ที่ตรงกับรายการในกล่องจดหมาย  

4. TrustScore จะกําหนดว่ารายการนั้นถูกเพิ่มหรือไม่ เหตุการณ์จะถูกเพิ่มเฉพาะเมื่อ TrustScore = "เชื่อถือ"

คุณสมบัติ Dm หรือ Dmarc ซึ่งอยู่ในส่วนหัวของข้อความ

เมื่อต้องการดูคุณสมบัติเหล่านี้:

**มุมมองเดสก์ท็อป**

- เปิดรายการ
- แฟ้ม -> คุณสมบัติ -> ส่วนหัวอินเทอร์เน็ต

หรือ

**Mfcmapi**

- นําทางไปยังรายการในกล่องจดหมาย
- มองหาPR_TRANSPORT_MESSAGE_HEADERS_W

คุณสมบัติเหล่านี้จะถูกกําหนด และบันทึกในระหว่างการขนส่งและสายงานการผลิต สําหรับการแก้ไขปัญหาเพิ่มเติม คุณอาจต้องติดตามด้วยการสนับสนุนการขนส่งเกี่ยวกับความล้มเหลวใน SPF, DKIM และ DMARC