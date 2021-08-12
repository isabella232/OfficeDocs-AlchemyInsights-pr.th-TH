---
title: แก้ไขปัญหารหัสข้อผิดพลาดการรับรองความถูกต้องและการอนุญาต Azure AD (AADSTS)
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
ms.openlocfilehash: ac25548b0110834c877ae53be097d6b6c0f13c4091040a901abd56fb2a3cbba3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939974"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a>แก้ไขปัญหารหัสข้อผิดพลาดการรับรองความถูกต้องและการอนุญาต Azure AD (AADSTS)

เมื่อต้องการแก้ไขการรับรองความถูกต้อง AAD และรหัสข้อผิดพลาดการรับรองความถูกต้อง (AADSTS) ให้ปฏิบัติตามขั้นตอนที่แนะนาต่อไปนี้:

1. **การจัดการรหัสข้อผิดพลาดในแอปพลิเคชันของคุณ**

- ข้อ **กําหนดเฉพาะ OAuth2.0** ให้แนวทางเกี่ยวกับวิธีการ https://tools.ietf.org/html/rfc6749#section-5.2 จัดการกับข้อผิดพลาดระหว่างการรับรองความถูกต้องโดยใช้ส่วนข้อผิดพลาดของการตอบกลับข้อผิดพลาด

    - **ข้อผิดพลาด**: สตริงรหัสข้อผิดพลาดที่สามารถใช้ในการจัดประเภทข้อผิดพลาดที่เกิดขึ้น และควรใช้เพื่อตอบสนองกับข้อผิดพลาด
    - เขตข้อมูล **ข้อผิดพลาด** มีค่าที่เป็นไปได้หลายค่า - ตรวจทานลิงก์คู่มือโพรโทคอลและข้อเพาะของ OAuth 2.0 เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดที่เฉพาะเจาะจงและวิธีการตอบสนองต่อข้อผิดพลาดเหล่านั้น

- นี่คือตัวอย่างการตอบกลับข้อผิดพลาด:
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
2. **ข้อมูลรหัสข้อผิดพลาดปัจจุบันของการค้นหา**

- รหัสข้อผิดพลาดและข้อความอาจมีการเปลี่ยนแปลง ดูข้อมูลล่าสุด ให้ดูหน้าเพื่อค้นหารายละเอียดข้อผิดพลาด AADSTS การแก้ไข และการแก้ไขปัญหาชั่วคราว https://login.microsoftonline.com/error ที่แนะนว
- คุณยังสามารถค้นหาและแก้ไขปัญหารหัสข้อผิดพลาด[AADSTS ที่แสดง](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes)อยู่ในบทความ รหัสข้อผิดพลาด[การรับรองความถูกต้องและการอนุญาต Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application)

3. **รับความช่วยเหลือ**

- [ตัวเลือกการสนับสนุนและวิธีใช้](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) ของนักพัฒนา - ถ้าคุณต้องการคําตอบของคําถามหรือความช่วยเหลือในการแก้ไขปัญหาที่ไม่ได้กล่าวถึงในเอกสารของเรา อาจถึงเวลาที่จะติดต่อผู้เชี่ยวชาญเพื่อขอความช่วยเหลือ บทความนี้มีคําแนะแพลตฟอร์มข้อมูลประจําตัวของ Microsoftตอบของคําถามของคุณ








