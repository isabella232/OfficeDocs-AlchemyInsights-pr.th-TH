---
title: ไม่สามารถเข้าสู่ระบบทีมได้เนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 649124db135805d8101b43dbead63860d36853ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799979"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>ไม่สามารถเข้าสู่ระบบทีมได้เนื่องจากข้อผิดพลาด autologon microsoftazuread-sso dot com: 443

ถ้ามีการเปิดใช้งาน SSO อย่างราบรื่นเป็นการรับรองความถูกต้องของ O365 URL "autologon.microsoftazuread-sso.com" อาจจำเป็นต้องเพิ่มลงในอินทราเน็ตไซต์  ถ้ามีการเพิ่มไปยังไซต์ที่เชื่อถือได้ก่อนหน้านี้และ SSO ที่ราบรื่นถูกใช้งานอยู่จะถูกเอาออกจากไซต์ที่เชื่อถือได้

โปรดตรวจทาน[รายการตรวจสอบการแก้ไขปัญหาของ SSO ที่ราบรื่น](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)

ทำตามขั้นตอนต่อไปนี้เพื่อเพิ่ม URL ลงในรายการไซต์อินทราเน็ต:

1. เปิด Internet Explorer ด้วยการคลิกปุ่ม**เริ่ม** ในกล่องค้นหาให้พิมพ์ Internet Explorer จากนั้นในรายการผลลัพธ์ให้คลิก**Internet Explorer**
2. คลิก**เครื่องมือ**แล้วคลิก**ตัวเลือกอินเทอร์เน็ต**
3. คลิกแท็บ**ความปลอดภัย**
4. ในตอนนี้ให้คลิกที่**ไซต์อินทราเน็ตเฉพาะ**ที่จากนั้นคลิกที่ปุ่ม**ไซต์**แล้วกดปุ่ม**ขั้นสูง**
5. ใส่ URL ของเว็บไซต์แล้วคลิก**เพิ่ม**
6. เมื่อคุณดำเนินการเสร็จสิ้นแล้วให้คลิก**ปิด**

สำหรับข้อมูลเพิ่มเติมให้ดูที่ [เอกสารประกอบสำหรับการปรับใช้ SSO อย่างราบรื่นสำหรับ O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (รวมถึงกระบวนการที่ใช้นโยบายเพื่อเพิ่ม URL ลงในไซต์อินทราเน็ตในขั้นตอนที่ 3)
