---
title: แก้ไขปัญหารหัสข้อผิดพลาดการรับรองความถูกต้องของ Azure AD และการอนุญาต (AADSTS)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037841"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>แก้ไขปัญหารหัสข้อผิดพลาดการรับรองความถูกต้องของ Azure AD และการอนุญาต (AADSTS)

เมื่อต้องการแก้ไขการรับรองความถูกต้อง AAD และรหัสข้อผิดพลาดการรับรองความถูกต้อง (AADSTS) ให้ปฏิบัติตามขั้นตอนที่แนะนาต่อไปนี้:

1. **การจัดการรหัสข้อผิดพลาดในแอปพลิเคชันของคุณ**

- ข้อ **กําหนด OAuth2.0** ให้แนวทางเกี่ยวกับวิธีการ https://tools.ietf.org/html/rfc6749#section-5.2 จัดการกับข้อผิดพลาดระหว่างการรับรองความถูกต้องโดยใช้ส่วนข้อผิดพลาดของการตอบกลับข้อผิดพลาด

    - **ข้อผิดพลาด**: สตริงรหัสข้อผิดพลาดที่สามารถใช้เพื่อจัดประเภทข้อผิดพลาดที่เกิดขึ้น และควรใช้เพื่อตอบสนองต่อข้อผิดพลาด
    - เขตข้อมูล **ข้อผิดพลาด** มีค่าที่เป็นไปได้หลายค่า - ตรวจทานลิงก์คู่มือโพรโทคอลและข้อเฉพาะเจาะจง OAuth 2.0 เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดที่เฉพาะเจาะจงและวิธีการตอบสนองต่อข้อผิดพลาดเหล่านั้น

- นี่คือตัวอย่างการตอบสนองข้อผิดพลาด:
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. **ค้นหาข้อมูลรหัสข้อผิดพลาดปัจจุบัน**

- รหัสข้อผิดพลาดและข้อความอาจเปลี่ยนแปลงได้ ดูข้อมูลล่าสุดที่หน้าเพื่อค้นหา https://login.microsoftonline.com/error รายละเอียดข้อผิดพลาด AADSTS การแก้ไข และการแก้ไขปัญหาชั่วคราวที่แนะน
- คุณยังสามารถค้นหาและแก้ไขปัญหารหัสข้อผิดพลาด[AADSTS ที่แสดง](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)อยู่ในบทความ การรับรองความถูกต้อง[Azure AD และรหัสข้อผิดพลาดการอนุญาต](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **ดูวิธีใช้**

- [ตัวเลือกการสนับสนุนและวิธีใช้](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) ของนักพัฒนา - ถ้าคุณต้องการคําตอบของคําถามหรือความช่วยเหลือในการแก้ไขปัญหาที่ไม่ครอบคลุมอยู่ในเอกสารประกอบของเรา อาจถึงเวลาที่จะติดต่อผู้เชี่ยวชาญเพื่อขอความช่วยเหลือ บทความนี้มีคําแนะนเกี่ยวกับการรับคําตอบของคําถามของคุณเมื่อคุณพัฒนาแอปที่รวมเข้ากับแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft








