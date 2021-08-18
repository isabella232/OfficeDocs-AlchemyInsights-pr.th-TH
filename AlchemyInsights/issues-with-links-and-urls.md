---
title: ปัญหาเกี่ยวกับลิงก์และ URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321926"
---
# <a name="issues-with-links-and-urls"></a>ปัญหาเกี่ยวกับลิงก์และ URL

การเปลี่ยนเส้นทาง URL ของ URI/การตอบกลับ (นิพจน์ทั้งสองรายการสามารถสลับกันได้) คือ URL แพลตฟอร์มข้อมูลประจําตัวของ Microsoftเพื่อส่งกลับโทเค็นที่ร้องขอโดยแอป หากต้องการข้อมูลเกี่ยวกับ URL เหล่านี้ โปรดดูบทความต่อไปนี้:

- [กระแสการรับรองความถูกต้องและสถานการณ์สมมติของ](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) แอปพลิเคชัน - ข้อมูลเกี่ยวกับ URI เปลี่ยนเส้นทาง **ในหน้าการลงทะเบียน** แอปของแต่ละสถานการณ์
- [เปลี่ยนเส้นทางข้อจํากัดและข้อจํากัดของ URL ของ URI/การตอบกลับ](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**ฉันไม่ทราบวิธีการลงทะเบียน URI เปลี่ยนเส้นทางที่ถูกต้อง / ตอบกลับ URL ของแอปของฉัน**

เมื่อคุณลงชื่อเข้าใช้ด้วยแอปพลิเคชันที่คุณพัฒนา ถ้ากล่องโต้ตอบลงชื่อเข้าใช้แสดง **AADSTS50011: URL <your app ID>** ตอบกลับที่ระบุในการร้องขอไม่ตรงกับ URL ตอบกลับที่กําหนดค่าไว้ให้กับแอปพลิเคชัน คุณจะต้องเพิ่มไปยังการลงทะเบียนแอปพลิเคชันของคุณ การเปลี่ยนเส้นทาง URI ที่โค้ดของคุณใช้ในการร้องขอโทเค็นไปยัง แพลตฟอร์มข้อมูลประจําตัวของ Microsoft

เมื่อต้องการเพิ่ม URL ตอบกลับ ให้ไปที่แท็บ **การรับรองความถูก** ต้อง ในหน้า **การลงทะเบียน** แอปพลิเคชันในพอร์ทัล Azure และเพิ่มรายการในส่วน **URI เปลี่ยนเส้นทาง** ค่าที่คุณต้องใส่จะขึ้นอยู่กับชนิดของแอปพลิเคชันที่คุณอยู่ ตามที่อธิบายไว้ด้านล่าง:

- For single-page applications and web apps, the reply URL is a URL in your application. ดู [การลงทะเบียนแอปพลิเคชันหน้าเว็บเดียว](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) หรือ [ลงทะเบียนแอปบนเว็บโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- For desktop apps, the value that you need to choose depends on:
    - แพลตฟอร์ม (MacOS แตกต่างจาก Windows หรือ Linux)
    - วิธีรับโทเค็น (แบบโต้ตอบได้กับโฟลว์รหัสอุปกรณ์ ที่มีการรับรองความถูกต้องแบบรวม Windows [IWA] หรือด้วยชื่อผู้ใช้/รหัสผ่าน)
    For details, see Desktop [apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- For mobile applications, the redirect URI depends on:
    - แพลตฟอร์ม (iOS/Android/UWP)
    - ข้อมูลที่ใช้ในการสร้างแอปของคุณ เช่น Bundle ID ใน iOS และชื่อแพคเกจและแฮชลายเซ็นบน Android การลงทะเบียนแอปพอร์ทัล Azure จะช่วยคุณได้ โปรดดูรายละเอียดที่[การกําหนดค่าแพลตฟอร์มและเปลี่ยนเส้นทาง URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)

**หมายเหตุ**: Web API และวิธีที่เงียบบางวิธีในการรับโทเค็น (IWA และชื่อผู้ใช้/รหัสผ่าน) ไม่ต้องมี URI การเปลี่ยนเส้นทาง

**ฉันได้ปรับใช้แอปพลิเคชันบนเว็บของฉัน และเมื่อฉันทดสอบแอปที่ปรับใช้ ฉันได้รับข้อความตอบกลับ URL ที่ไม่ตรงกัน**

เพิ่ม URI การเปลี่ยนเส้นทางของทุกที่ตั้งที่คุณปรับใช้แอปพลิเคชันบนเว็บของคุณ หากต้องการข้อมูลเพิ่มเติม โปรดดู[ลงทะเบียนแอปบนเว็บโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)

**หมายเหตุ**: เพิ่ม URI การเปลี่ยนเส้นทางไปยังสถานที่หนึ่งทันทีหลังจากที่คุณได้ปรับใช้แอปพลิเคชันในที่นั้นแล้ว

**ฉันไม่สามารถลงทะเบียน URL ตอบกลับได้มากพอ**

คุณเป็น ISV และมี URI เปลี่ยนเส้นทางหนึ่งหรือหลายรายการกับลูกค้าทุกคนของคุณ คุณต้องการโยกย้ายจาก ADAL/Azure AD v1.0 ไปยัง MSAL/the แพลตฟอร์มข้อมูลประจําตัวของ Microsoft และคุณมีจํานวน URL การเปลี่ยนเส้นทาง[สูงสุด](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) เมื่อต้องการแก้ไขปัญหานี้ [ให้เพิ่ม URI เปลี่ยนเส้นทางไปยังหลักของ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) บริการที่สอดคล้องกับลูกค้าแต่ละรายของคุณ
