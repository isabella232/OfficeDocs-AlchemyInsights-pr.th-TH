---
title: ไม่สามารถเข้าสู่ระบบTeamsเนื่องจาก autologon.microsoftazuread-sso.com:443
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
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038419"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>ไม่สามารถเข้าสู่ระบบในTeamsเนื่องจากข้อผิดพลาด autologon.microsoftazuread-sso dot com:443

ถ้าเปิดใช้งาน SSO อย่างราบรื่นเป็นการรับรองความถูกต้อง O365 URL "autologon.microsoftazuread-sso.com" อาจจะถูกเพิ่มลงในไซต์อินทราเน็ต  ถ้าก่อนหน้านี้ถูกเพิ่มลงในไซต์ที่เชื่อถือได้และใช้ SSO อย่างราบรื่น อยู่ ควรเอา SSO ออกจากไซต์ที่เชื่อถือได้

โปรดตรวจทานรายการ [ตรวจสอบการแก้ไขปัญหา SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)อย่างราบรื่น

ให้ปฏิบัติตามขั้นตอนเหล่านี้เพื่อเพิ่ม URL ลงในรายการไซต์อินทราเน็ต

1. เปิด Internet Explorer **โดยการคลิกปุ่ม** เริ่ม ในกล่องค้นหา ให้พิมพ์ Internet Explorer จากนั้นในรายการผลลัพธ์ ให้คลิก **Internet Explorer**
2. **คลิก** เครื่องมือ แล้วคลิก **ตัวเลือก** อินเทอร์เน็ต
3. **คลิกแท็บ** ความปลอดภัย
4. ในตอนนี้ **ให้คลิกที่ ไซต์อินทราเน็ต** เฉพาะที่ จากนั้นคลิก **ปุ่ม** ไซต์ **จากนั้นคลิกปุ่ม** ขั้นสูง
5. ใส่ URL ของเว็บไซต์ **แล้วคลิก** เพิ่ม
6. เมื่อเสร็จแล้ว **ให้คลิก** ปิด

For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes policy-based process to add a URL to Intranet Sites in step 3).
