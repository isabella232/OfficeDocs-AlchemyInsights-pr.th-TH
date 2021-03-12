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
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707901"
---
# <a name="issues-with-links-and-urls"></a>ปัญหาเกี่ยวกับลิงก์และ URL

URL การเปลี่ยนเส้นทาง URI/การตอบกลับ (ทั้งสองนิพจน์สามารถสลับกันได้) คือ URL ที่ใช้โดยแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft เพื่อส่งกลับโทเค็นที่ร้องขอโดยแอป ดูบทความต่อไปนี้เพื่อดูข้อมูลเกี่ยวกับ URL เหล่านี้:

- [การรับรองความถูกต้องโฟลว์และสถานการณ์สมมติ](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) ของแอปพลิเคชัน - ข้อมูลเกี่ยวกับ URI การเปลี่ยนเส้นทาง **ในหน้าการลงทะเบียน** แอปของแต่ละสถานการณ์
- [การเปลี่ยนเส้นทางข้อจํากัดและข้อจํากัดของ URL URI/การตอบกลับ](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**ฉันไม่ทราบวิธีการลงทะเบียน URI เปลี่ยนเส้นทางที่ถูกต้อง / URL ตอบกลับของแอปของฉัน**

เมื่อคุณลงชื่อเข้าใช้ด้วยแอปพลิเคชันที่คุณพัฒนา ถ้ากล่องโต้ตอบลงชื่อเข้าใช้แสดง **AADSTS50011: URL <your app ID>** ตอบกลับที่ระบุในการร้องขอไม่ตรงกับ URL ตอบกลับที่กําหนดค่าไว้ให้กับแอปพลิเคชัน คุณจะต้องเพิ่มไปยังการลงทะเบียนแอปพลิเคชันของคุณ การเปลี่ยนเส้นทาง URI ที่โค้ดของคุณใช้ในการร้องขอโทเค็นไปยังแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft

เมื่อต้องการเพิ่ม URL ตอบกลับ ให้ไปที่แท็บ **การรับรองความถูก****ต้องในหน้าการลงทะเบียน** แอปพลิเคชันในพอร์ทัล Azure และเพิ่มรายการในส่วน **URI การ** เปลี่ยนเส้นทาง ค่าที่คุณต้องใส่จะขึ้นอยู่กับชนิดของแอปพลิเคชันที่คุณสร้าง ตามที่อธิบายไว้ด้านล่าง:

- For single-page applications and web apps, the reply URL is a URL in your application. ดู [การลงทะเบียนแอปพลิเคชันหน้าเดียว](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) หรือ [ลงทะเบียนแอปบนเว็บโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- ในแอปบนเดสก์ท็อป ค่าที่คุณต้องเลือกจะขึ้นอยู่กับสิ่งต่อไปนี้
    - แพลตฟอร์ม (MacOS แตกต่างจาก Windows หรือ Linux)
    - วิธีที่คุณรับโทเค็น (แบบโต้ตอบด้วยลโฟลว์รหัสอุปกรณ์ด้วยการรับรองความถูกต้องของ Windows แบบรวม [IWA] หรือด้วยชื่อผู้ใช้/รหัสผ่าน)
    For details, see [Desktop apps - การลงทะเบียนแอป - เปลี่ยนเส้นทาง URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- For mobile applications, the redirect URI depends on:
    - แพลตฟอร์ม (iOS/Android/UWP)
    - ข้อมูลที่ใช้ในการสร้างแอปของคุณ เช่น Bundle ID ใน iOS และชื่อแพคเกจและแฮชลายเซ็นบน Android การลงทะเบียนแอปพอร์ทัล Azure จะช่วยคุณได้ For details, see [platform configuration and redirect URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> API เว็บและวิธีที่เงียบบางวิธีในการรับโทเค็น (IWA และชื่อผู้ใช้/รหัสผ่าน) ไม่ต้องมี URI การเปลี่ยนเส้นทาง

**ฉันได้ปรับใช้แอปพลิเคชันบนเว็บของฉันและเมื่อฉันทดสอบแอปที่ปรับใช้ ฉันได้รับข้อความตอบกลับ URL ที่ไม่ตรงกัน**

เพิ่ม URI เปลี่ยนเส้นทางของทุกที่ตั้งที่คุณปรับใช้แอปพลิเคชันบนเว็บของคุณ ดูข้อมูลเพิ่มเติมในการลงทะเบียน[แอปบนเว็บโดยใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)

> [!NOTE]
> เพิ่ม URI เปลี่ยนเส้นทางไปยังสถานที่หนึ่งทันทีหลังจากที่คุณได้ปรับใช้แอปพลิเคชันที่สถานที่นั้นแล้ว

**ฉันไม่สามารถลงทะเบียน URL ตอบกลับได้มากพอ**

คุณเป็น ISV และมี URI เปลี่ยนเส้นทางหนึ่งหรือหลายรายการกับลูกค้าของคุณทุกคน คุณต้องการโยกย้ายจาก ADAL/Azure AD v1.0 ไปยัง MSAL/แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft และคุณมีจํานวนสูงสุดในการเปลี่ยนเส้นทาง[URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) เมื่อต้องการแก้ไขปัญหานี้ [ให้เพิ่ม URI เปลี่ยนเส้นทางไปยังบริการ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) หลักที่สอดคล้องกับลูกค้าของคุณแต่ละรายการ
