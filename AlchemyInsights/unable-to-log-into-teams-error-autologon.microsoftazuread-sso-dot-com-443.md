---
title: ไม่สามารถเข้าสู่ระบบ Teams เนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932286"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>ไม่สามารถเข้าสู่ระบบทีมได้เนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso ดอทคอม:443

ถ้า SSO แบบไม่มีรอยต่อถูกเปิดใช้งานเป็นการรับรองความถูกต้องของ O365, URL "autologon.microsoftazuread-sso.com" อาจจําเป็นต้องเพิ่มไปยังไซต์อินทราเน็ต  ถ้าก่อนหน้านี้ได้ถูกเพิ่มไปยังไซต์ที่เชื่อถือได้และ SSO แบบไม่มีรอยต่อถูกใช้งาน

โปรดตรวจสอบ[รายการตรวจสอบการแก้ปัญหา SSO ที่ไร้รอยต่อ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)

ทําตามขั้นตอนเหล่านี้เพื่อเพิ่ม URL ลงในรายการไซต์อินทราเน็ต:

1. เปิด Internet Explorer ด้วยการคลิกปุ่ม**เริ่ม** ในกล่องค้นหา ให้พิมพ์ Internet Explorer จากนั้นในรายการผลลัพธ์ ให้คลิก**Internet Explorer**
2. คลิก**เครื่องมือ**แล้วคลิก**ตัวเลือกอินเทอร์เน็ต**
3. คลิกการ**การรักษาความปลอดภัย**แท็บ
4. ตอนนี้คลิกที่**เว็บไซต์อินทราเน็ตท้องถิ่น**แล้วคลิกที่ปุ่ม**เว็บไซต์**แล้วปุ่ม**ขั้นสูง**
5. ป้อน URL ของเว็บไซต์ และคลิก**เพิ่ม**
6. เมื่อคุณดําเนินการเสร็จสิ้นแล้ว ให้คลิก**ปิด**

สําหรับข้อมูลเพิ่มเติม ให้ดู[เอกสารประกอบสําหรับการปรับใช้ SSO แบบไม่มีรอยต่อสําหรับ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (รวมถึงกระบวนการตามนโยบายเพื่อเพิ่ม URL ไปยังไซต์อินทราเน็ตในขั้นตอนที่ 3)
