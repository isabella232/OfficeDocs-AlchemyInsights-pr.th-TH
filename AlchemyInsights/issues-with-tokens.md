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
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917216"
---
# <a name="issues-with-tokens"></a>ปัญหาเกี่ยวกับโทเค็น

เมื่อต้องการจัดการปัญหาที่เกี่ยวข้องกับโทเค็นคุณสามารถทำตามขั้นตอนต่อไปนี้:

1. คุณสามารถระบุอายุการใช้งานของการเข้าถึง ID หรือโทเค็น SAML ที่ออกโดยแพลตฟอร์มข้อมูลประจำตัวของไมโครซอฟท์ คุณสามารถตั้งค่าการหมดอายุของโทเค็นสำหรับแอปทั้งหมดในองค์กรของคุณสำหรับแอปพลิเคชันแบบหลายผู้เช่า (หลายองค์กร) หรือสำหรับบริการหลักที่เฉพาะเจาะจงในองค์กรของคุณ สำหรับข้อมูลเพิ่มเติมให้ดูที่การกำหนดค่าของ[โทเค็นที่กำหนดค่าไว้ใน Microsoft identity platform (ตัวอย่าง)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
2. โทเค็นการเข้าถึงจะเปิดใช้งานไคลเอ็นต์ในการโทรที่มีการป้องกันเว็บ APIs อย่างปลอดภัยและใช้งานเว็บ APIs เพื่อดำเนินการรับรองความถูกต้องและการอนุญาต ตามข้อกำหนดของ OAuth โทเค็นการเข้าถึงจะเป็นสตริงตัวทึบโดยไม่มีรูปแบบชุด-ผู้ให้บริการข้อมูลเฉพาะตัว (IDPs) ใช้ Guid ที่ผู้ใช้อื่นใช้งาน blobs ที่เข้ารหัสลับ แพลตฟอร์มสำหรับข้อมูลเฉพาะตัวของ Microsoft ใช้รูปแบบโทเค็นการเข้าถึงที่หลากหลายขึ้นอยู่กับการกำหนดค่าของ API ที่ยอมรับโทเค็น เมื่อต้องการเรียนรู้วิธีที่ API ของคุณสามารถตรวจสอบและใช้การอ้างสิทธิ์ภายในโทเค็นการเข้าถึงให้ดูที่[โทเค็นการเข้าถึงแพลตฟอร์มสำหรับข้อมูลประจำตัวของไมโครซอฟท์](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)
3. ไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) สนับสนุนการทำงานของการรับรองความถูกต้องหลายขั้นตอนในการใช้งานในสถานการณ์สมมติ สำหรับข้อมูลเพิ่มเติมให้ดูที่[ขั้นตอนการรับรองความถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)
4. คุณสามารถใช้รหัสการตรวจสอบสิทธิ์ของ OAuth ๒.๐ในแอปที่ติดตั้งบนอุปกรณ์เพื่อเข้าถึงทรัพยากรที่มีการป้องกันเช่นเว็บ APIs การใช้ Microsoft identity platform การใช้งานของ OAuth ๒.๐คุณสามารถเพิ่มการเข้าสู่ระบบและการเข้าถึง API ไปยังแอปสำหรับอุปกรณ์เคลื่อนที่และเดสก์ท็อปของคุณได้ ให้ดูที่ [แพลตฟอร์มสำหรับข้อมูลประจำตัวของ Microsoft และการรับส่งข้อมูลรหัสการตรวจสอบ OAuth ๒.๐](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) สำหรับวิธีการทำงานของโปรแกรมโดยตรงกับโพรโทคอลในแอปพลิเคชันของคุณโดยใช้ภาษาใดๆ
5. OpenID Connect (OIDC) เป็นโพรโทคอลการรับรองความถูกต้องที่สร้างขึ้นบน OAuth ๒.๐ที่คุณสามารถใช้เพื่อลงชื่อเข้าใช้ในแอปพลิเคชันได้อย่างปลอดภัย เมื่อคุณใช้ Microsoft identity platform ของจุดสิ้นสุดการดำเนินการของ OpenID การเชื่อมต่อคุณสามารถเพิ่มการเข้าสู่ระบบและการเข้าถึง API ของคุณไปยังแอปของคุณได้ [Microsoft identity platform และโพรโทคอลการเชื่อมต่อ OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) จะแสดงวิธีการทำงานที่ไม่ขึ้นกับภาษาและอธิบายวิธีการส่งและรับข้อความ HTTP โดยไม่ต้องใช้ไลบรารีแหล่งข้อมูลที่เปิดอยู่ของ microsoft
    - จุดสิ้นสุดของ UserInfo เป็นส่วนหนึ่งของมาตรฐาน OIDC ที่ได้รับการออกแบบมาเพื่อส่งกลับการอ้างสิทธิ์เกี่ยวกับผู้ใช้ที่ได้รับการรับรองความถูกต้อง สำหรับข้อมูลเพิ่มเติมให้ดูที่จุดสิ้นสุดของ[Microsoft identity Platform UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)
    - การ [โทรผ่านเว็บ API ในเว็บแอปโดยใช้ AZURE ad และ OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) จะแสดงวิธีการสร้างแอปพลิเคชัน MVC บนเว็บที่ใช้ azure AD สำหรับการลงชื่อเข้าใช้โดยใช้การเชื่อมต่อโพรโทคอล OpenID แล้วโทรผ่านเว็บ API ภายใต้ข้อมูลเฉพาะตัวของผู้ใช้ที่ลงชื่อเข้าใช้โดยใช้โทเค็น๒.๐ ตัวอย่างนี้ใช้ OpenID เชื่อมต่อ ASP .Net OWIN และ ADAL .Net
6. [กำหนดค่าแอปพลิเคชันเพื่อแสดงเว็บ api](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -ใน quickstart นี้คุณจะลงทะเบียนเว็บ Api ด้วย Microsoft identity platform และแสดงแอปพลิเคชันไคลเอ็นต์โดยการเพิ่มขอบเขตตัวอย่าง ด้วยการลงทะเบียนเว็บ API ของคุณและเปิดเผยข้อมูลผ่านขอบเขตคุณสามารถให้สิทธิ์การเข้าถึงทรัพยากรของผู้ใช้ที่ได้รับอนุญาตและแอปพลิเคชันไคลเอ็นต์ที่เข้าถึง API ของคุณได้
7. ใน Azure Active Directory B2C (Azure AD B2C) การไหลของเจ้าของทรัพยากรข้อมูลประจำตัว (ROPC) คือการไหลของการรับรองความถูกต้องของมาตรฐาน OAuth ในขั้นตอนนี้แอปพลิเคชันหรือที่เรียกอีกอย่างว่าบริษัท relying ให้แลกเปลี่ยนข้อมูลประจำตัวที่ถูกต้องสำหรับโทเค็น ข้อมูลประจำตัวมี ID ผู้ใช้และรหัสผ่าน โทเค็นที่ส่งกลับเป็นโทเค็น ID โทเค็นการเข้าถึงและโทเค็นการรีเฟรช สำหรับข้อมูลเพิ่มเติมให้ดู [ที่การตั้งค่าการไหลของข้อมูลประจำตัวของเจ้าของทรัพยากรใน B2C Azure active](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow)directory 

