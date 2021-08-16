---
title: ปัญหาเกี่ยวกับโทเค็น
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: a4e99f1f80df601ddf53498d9a8323790fc52a50b2e067f17429da0bf6a03c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067463"
---
# <a name="issues-with-tokens"></a>ปัญหาเกี่ยวกับโทเค็น

เมื่อต้องการจัดการปัญหาที่เกี่ยวข้องกับโทเค็น คุณสามารถปฏิบัติตามขั้นตอนต่อไปนี้:

1. คุณสามารถระบุอายุการใช้งานของโทเค็นการเข้าถึง ID หรือ SAML ที่ออกให้โดยแพลตฟอร์มข้อมูลประจําตัวของ Microsoftได้ คุณสามารถตั้งค่าอายุการใช้งานโทเค็นของแอปทั้งหมดในองค์กรของคุณ, แอปพลิเคชันแบบหลายผู้เช่า (หลายองค์กร) หรือแอปพลิเคชันหลักบริการเฉพาะในองค์กรของคุณได้ For more information, see [Configurable token lifetimes in แพลตฟอร์มข้อมูลประจําตัวของ Microsoft (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. โทเค็นการเข้าถึงจะเปิดใช้งานไคลเอ็นต์เพื่อเรียกใช้ API เว็บที่มีการป้องกันอย่างปลอดภัย และถูกใช้โดย API เว็บเพื่อรับรองความถูกต้องและการอนุญาต ตามข้อมูลเฉพาะของ OAuth โทเค็นการเข้าถึงเป็นสตริงสีทึบโดยไม่มีรูปแบบที่ตั้งค่า - ผู้ให้บริการข้อมูลเฉพาะตัว (IDP) บางรายจะใช้ GUIDs ส่วนอื่นๆ จะใช้ Blob ที่เข้ารหัสลับ กลุ่มแพลตฟอร์มข้อมูลประจําตัวของ Microsoftรูปแบบโทเค็นการเข้าถึงที่หลากหลาย ขึ้นอยู่กับการกําหนดค่า API ที่ยอมรับโทเค็น เมื่อต้องการเรียนรู้วิธีที่ API ของคุณสามารถตรวจสอบและใช้การอ้างสิทธิ์ภายในโทเค็นการเข้าถึง[แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโทเค็นการเข้าถึง](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)
3. ไลบรารี Microsoft Authentication Library (MSAL) สนับสนุนโฟลว์การรับรองความถูกต้องหลายอย่างเพื่อใช้ในสถานการณ์ของแอปพลิเคชันต่างๆ For more information, see [Authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. การอนุญาตรหัส OAuth 2.0 สามารถใช้ในแอปที่ติดตั้งบนอุปกรณ์เพื่อเข้าถึงทรัพยากรที่ได้รับการป้องกัน เช่น API เว็บ ด้วยการใช้แพลตฟอร์มข้อมูลประจําตัวของ Microsoft OAuth 2.0 คุณสามารถเพิ่มการลงชื่อเข้าใช้และการเข้าถึง API ไปยังแอปบนอุปกรณ์เคลื่อนที่และเดสก์ท็อปของคุณ ดู[แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโฟลว์รหัสการรับรองความถูกต้อง แพลตฟอร์มข้อมูลประจําตัวของ Microsoft OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token)เพื่อดูวิธีการเขียนโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณโดยใช้ภาษาใดก็ได้
5. OpenID เชื่อมต่อ (OIDC) คือโพรโทคอลการรับรองความถูกต้องที่สร้างขึ้นบน OAuth 2.0 ที่คุณสามารถใช้เพื่อลงชื่อเข้าใช้แอปพลิเคชันของผู้ใช้อย่างปลอดภัย เมื่อคุณใช้การปรับใช้ แพลตฟอร์มข้อมูลประจําตัวของ Microsoft OpenID เชื่อมต่อของจุดสิ้นสุดการลงชื่อเข้าใช้ คุณสามารถเพิ่มการเข้าถึงการลงชื่อเข้าใช้และ API ไปยังแอปของคุณ [แพลตฟอร์มข้อมูลประจําตัวของ Microsoftและโพรโทคอล OpenID เชื่อมต่อ](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request)แสดงวิธีการแยกภาษาและอธิบายวิธีการส่งและรับข้อความ HTTP โดยไม่ต้องใช้ไลบรารีโอเพนซอร์สของไมโครซอฟท์
    - จุดสิ้นสุด UserInfo เป็นส่วนหนึ่งของมาตรฐาน OIDC ซึ่งออกแบบมาเพื่อส่งกลับการอ้างสิทธิ์เกี่ยวกับผู้ใช้ที่ได้รับการรับรองความถูกต้อง For more information, see[แพลตฟอร์มข้อมูลประจําตัวของ Microsoft UserInfo endpoint](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - ตัวอย่างการโทรผ่านเว็บ API ในเว็บโดยใช้ Azure AD และ[OpenID เชื่อมต่อ](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/)แสดงวิธีการสร้างแอปพลิเคชันบนเว็บ MVC ที่ใช้ Azure AD เพื่อลงชื่อเข้าใช้โดยใช้โพรโทคอล OpenID เชื่อมต่อ แล้วเรียกใช้เว็บ API ภายใต้ข้อมูลเฉพาะตัวของผู้ใช้ที่ลงชื่อเข้าใช้โดยใช้โทเค็นที่ได้รับผ่าน OAuth 2.0 ตัวอย่างนี้ใช้ OpenID เชื่อมต่อ ASP .Net OWIN middleware และ ADAL .Net
6. [กําหนดค่าแอปพลิเคชันให้แสดง API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis)เว็บ - ในการเริ่มต้นใช้งานด่วนนี้ คุณลงทะเบียน API เว็บด้วยแพลตฟอร์มข้อมูลประจําตัวของ Microsoft และแสดงในแอปไคลเอ็นต์โดยการเพิ่มขอบเขตตัวอย่าง โดยการลงทะเบียน API บนเว็บของคุณและเปิดเผยผ่านขอบเขต คุณสามารถให้สิทธิ์การเข้าถึงทรัพยากรของผู้ใช้ที่ได้รับอนุญาตและแอปไคลเอ็นต์ที่เข้าถึง API ของคุณ
7. ใน Azure Active Directory B2C (Azure AD B2C) โฟลว์ข้อมูลรับรองความถูกต้องของรหัสผ่านเจ้าของทรัพยากร (ROPC) คือโฟลว์การรับรองความถูกต้องมาตรฐาน OAuth ในโฟลว์นี้ แอปพลิเคชันหรือที่เรียกว่าฝ่ายที่เกี่ยวข้อง แลกเปลี่ยนข้อมูลรับรองที่ถูกต้องของโทเค็น ข้อมูลรับรองจะมี ID ผู้ใช้และรหัสผ่าน โทเค็นที่ส่งกลับคือโทเค็น ID โทเค็นการเข้าถึง และโทเค็นรีเฟรช For more information, see [Set up a resource owner password credentials flow in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

