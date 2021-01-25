---
title: ปัญหาเกี่ยวกับลิงก์และ Url
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
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974756"
---
# <a name="issues-with-links-and-urls"></a>ปัญหาเกี่ยวกับลิงก์และ Url

การเปลี่ยนเส้นทาง Url URI/ตอบกลับ (ทั้งสองนิพจน์จะสามารถเปลี่ยนได้) คือ Url ที่ใช้โดยแพลตฟอร์มสำหรับข้อมูลเฉพาะตัวของ Microsoft เพื่อส่งกลับโทเค็นที่ร้องขอแอป สำหรับข้อมูลเกี่ยวกับ Url เหล่านี้ให้ดูบทความต่อไปนี้:

- [ขั้นตอนการรับรองความถูกต้องและสถานการณ์สมมติของแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -ข้อมูลเกี่ยวกับการเปลี่ยนเส้นทาง URIs ในหน้าการ **ลงทะเบียนแอปของ** แต่ละสถานการณ์
- [การเปลี่ยนเส้นทางข้อจำกัดและข้อจำกัดของ URL ของ URI/ตอบกลับ](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**ฉันไม่ทราบวิธีการลงทะเบียน URL URI/ตอบกลับที่ถูกเปลี่ยนเส้นทางขวาสำหรับแอปของฉัน**

เมื่อคุณลงชื่อเข้าใช้ด้วยแอปพลิเคชันที่คุณกำลังพัฒนาถ้ากล่องโต้ตอบการลงชื่อเข้าใช้แสดง **AADSTS50011: url ตอบกลับที่ระบุในการร้องขอไม่ตรง <your app ID> กับ url ตอบกลับที่กำหนดค่าไว้สำหรับแอปพลิเคชัน** คุณจะต้องเพิ่มลงในการลงทะเบียนแอปพลิเคชันของคุณ, URI การเปลี่ยนเส้นทางที่รหัสของคุณใช้ในการร้องขอโท

เมื่อต้องการเพิ่ม URL การตอบกลับให้ไปที่แท็บการ **รับรองความถูกต้อง** ในหน้าการ **ลงทะเบียนแอปพลิเคชัน** ของคุณในพอร์ทัล Azure และเพิ่มรายการในส่วนการ **เปลี่ยนเส้นทาง URIs** เปลี่ยนเส้นทาง URIs จะถูกพิมพ์ (เว็บหรืออุปกรณ์เคลื่อนที่/เดสก์ท็อป) ค่าที่คุณจำเป็นต้องใส่จะขึ้นอยู่กับชนิดของแอปพลิเคชันที่คุณกำลังสร้างตามที่อธิบายไว้ด้านล่าง:

- สำหรับแอปพลิเคชันหน้าเดียวและเว็บแอป URL ตอบกลับคือ URL ในแอปพลิเคชันของคุณ ดูการ [ลงทะเบียนแอปพลิเคชันหน้าเดียว](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) หรือ [ลงทะเบียนแอป web App โดยใช้ Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- สำหรับแอปเดสก์ท็อปค่าที่คุณจำเป็นต้องเลือกจะขึ้นอยู่กับ:
    - platform (MacOS จะแตกต่างจาก Windows หรือ Linux)
    - วิธีที่คุณได้รับโทเค็น (แบบโต้ตอบที่มีการทำงานของรหัสอุปกรณ์ที่มีการรับรองความถูกต้องของ Windows แบบรวม [IWA] หรือที่มีชื่อผู้ใช้/รหัสผ่าน)
    สำหรับรายละเอียดให้ดูที่การ [ลงทะเบียนแอปบนเดสก์ท็อป-การเปลี่ยนเส้นทาง URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- สำหรับแอปพลิเคชันมือถือ URI การเปลี่ยนเส้นทางจะขึ้นอยู่กับ:
    - platform (iOS/Android/UWP)
    - ข้อมูลที่ใช้ในการสร้างแอปของคุณเช่น ID bundle ใน iOS และชื่อแพคเกจและการแฮชสำหรับลายเซ็นบน Android การลงทะเบียนแอป Azure portal จะช่วยคุณได้ สำหรับรายละเอียดให้ดูที่[การกำหนดค่าของแพลตฟอร์มและการเปลี่ยนเส้นทาง URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)

> [!NOTE]
> เว็บ APIs และบางวิธีที่เงียบของการรับโทเค็น (IWA และชื่อผู้ใช้/รหัสผ่าน) ไม่จำเป็นต้องมี URI การเปลี่ยนเส้นทาง

**ฉันได้ปรับใช้แอปพลิเคชันเว็บของฉันและเมื่อฉันทดสอบแอปที่ปรับใช้แล้วฉันจะได้รับข้อความตอบกลับ url ที่ไม่ตรงกัน**

เพิ่มการเปลี่ยนเส้นทาง URIs สำหรับตำแหน่งที่ตั้งทั้งหมดที่คุณกำลังปรับใช้แอปพลิเคชันบนเว็บของคุณ สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ลงทะเบียนแอป web app โดยใช้ Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)

> [!NOTE]
> เพิ่มการเปลี่ยนเส้นทาง URI สำหรับตำแหน่งที่ตั้งทันทีหลังจากที่คุณได้ปรับใช้แอปพลิเคชันที่ตำแหน่งที่ตั้งนั้น

**ฉันไม่สามารถลงทะเบียน Url การตอบกลับเพียงพอ**

คุณเป็น ISV และมีการเปลี่ยนเส้นทาง URIs หนึ่งหรือหลายรายการสำหรับลูกค้าทุกรายของคุณ คุณต้องการโยกย้ายจาก ADAL/Azure AD v1.0 เป็น MSAL/Microsoft identity platform และคุณจะกด[จำนวนสูงสุดของการเปลี่ยนเส้นทาง URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) เมื่อต้องการแก้ไขปัญหานี้ให้ [เพิ่มการเปลี่ยนเส้นทาง URIs ไปยัง](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) การรักษาบริการที่สอดคล้องกับลูกค้าแต่ละรายของคุณ
