---
title: แก้ไขปัญหาโพรโทคอล OAuth 2.0 และ OpenID เชื่อมต่อ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921062"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>แก้ไขปัญหาโพรโทคอล OAuth 2.0 และ OpenID เชื่อมต่อ

เมื่อต้องการแก้ไขปัญหา OAuth 2.0 และ OpenID เชื่อมต่อ ให้ปฏิบัติตามขั้นตอนที่แนะนาต่อไปนี้:

ดูบทความต่อไปนี้ที่เกี่ยวข้องกับการกําหนดค่าและการแก้ไขปัญหา OAuth 2.0 และ OpenID เชื่อมต่อโพรโทคอลของคุณ:

- แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโฟลว์รหัสการรับรองความถูกต้อง [และ OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับ Code **Grant (PKCE)** ในแอปพลิเคชันของคุณโดยใช้ภาษาใดก็ได้
- [แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโฟลว์ข้อมูลรับรองความถูกต้องของไคลเอ็นต์ OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟลว์ **ข้อมูลรับรองไคลเอ็นต์** ในแอปพลิเคชันของคุณ
- [แพลตฟอร์มข้อมูลประจําตัวของ Microsoftข้อมูลรับรองรหัสผ่านเจ้าของทรัพยากรและ OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟลว์ **ROPC** ในแอปพลิเคชันของคุณ
    - ตัวเลือกแพลตฟอร์มข้อมูลประจําตัวของ Microsoftจะสนับสนุนเฉพาะ ROPC ผู้เช่า Azure AD เท่านั้น และไม่รองรับบัญชีส่วนบุคคล ซึ่งหมายความว่าคุณต้องใช้จุดสิ้นสุดเฉพาะผู้เช่า **https://login.microsoftonline.com/{TenantId_or_Name}) (** หรือ **จุดสิ้นสุด** องค์กร
    - บัญชีส่วนบุคคลที่ได้รับเชิญให้เป็นผู้เช่า Azure AD จะใช้งาน ROPC ไม่ได้
    - บัญชีที่มีรหัสผ่านไม่สามารถลงชื่อเข้าใช้ผ่าน ROPC ได้ ในสถานการณ์สมมตินี้ เราขอแนะนนะให้คุณใช้ขั้นตอนที่แตกต่างกันในแอปของคุณแทน
    - ถ้าผู้ใช้ต้องใช้ [การรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) เพื่อเข้าสู่ระบบแอปพลิเคชัน พวกเขาจะถูกบล็อก
    - ROPC ไม่ได้รับการสนับสนุนในสถานการณ์การ [ติดต่อกับภายนอก](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) แบบไฮบริด (ตัวอย่างเช่น Azure AD และ ADFS ที่ใช้ในการรับรองความถูกต้องของบัญชีภายในองค์กร) ถ้าผู้ใช้เปลี่ยนเส้นทางแบบเต็มหน้าไปยังผู้ให้บริการข้อมูลเฉพาะตัวภายในองค์กร Azure AD จะไม่สามารถทดสอบชื่อผู้ใช้และรหัสผ่านกับผู้ให้บริการข้อมูลเฉพาะตัวนั้น [อย่างไรก็ตาม การรับรองความถูกต้องแบบ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) พาส-พาส-พาสได้รับการสนับสนุนกับ ROPC
    - ข้อยกเว้นของสถานการณ์การติดต่อกับภายนอกแบบไฮบริดจะเป็นสิ่งต่อไปนี้: นโยบาย Home Realm Discovery ที่มี **การตั้งค่า AllowCloudPasswordValidation** **เป็น TRUE** จะเปิดใช้งานโฟลว์ ROPC เพื่อใช้งานกับผู้ใช้ภายนอกเมื่อซิงค์รหัสผ่านภายในองค์กรกับระบบคลาวด์ For more information, see [Enable direct ROPC authentication of federrated users for legacy applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [แพลตฟอร์มข้อมูลประจําตัวของ Microsoft และ OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟลว์ในนามของ **(OBO)** ในแอปพลิเคชันของคุณ
- [แพลตฟอร์มข้อมูลประจําตัวของ Microsoft OpenID เชื่อมต่อ -](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc)บทความนี้แสดงวิธีการใช้โพรโทคอล OpenID เชื่อมต่อ ที่เป็นอิสระของภาษา และอธิบายวิธีการส่งและรับข้อความ HTTP โดยไม่ต้องใช้ไลบรารีโอเพนซอร์สของไมโครซอฟท์

**เข้าถึงโทเค็น**

[แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโทเค็นการเข้าถึง](https://docs.microsoft.com/azure/active-directory/develop/access-tokens)- เรียนรู้วิธีที่ API ของคุณสามารถตรวจสอบและใช้การอ้างสิทธิ์ภายในโทเค็นการเข้าถึง เอกสารประกอบทั้งหมดในบทความนี้ ยกเว้นที่บันทึกจะใช้ได้กับโทเค็นที่ออกให้ API ที่คุณลงทะเบียนเท่านั้น ซึ่งจะไม่มีผลบังคับใช้กับโทเค็นที่ออกให้กับ API ที่ Microsoft เป็นเจ้าของ และไม่สามารถใช้โทเค็นเหล่านั้นเพื่อตรวจสอบวิธีที่ แพลตฟอร์มข้อมูลประจําตัวของ Microsoft จะออกโทเค็นให้กับ API ที่คุณสร้าง

**การกําหนดค่าแอปพลิเคชัน**

[การเปลี่ยนเส้นทางข้อจํากัดและข้อจํากัด URI (URL ตอบกลับ)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - เรียนรู้วิธีการกําหนดค่า URI การเปลี่ยนเส้นทาง (URL ตอบกลับ) ของคุณ การเปลี่ยนเส้นทาง URI หรือ URL ตอบกลับ คือที่ตั้งที่เซิร์ฟเวอร์การรับรองความถูกต้องส่งผู้ใช้เมื่อแอปได้รับอนุญาตและมอบรหัสการตรวจสอบหรือโทเค็นการเข้าถึงเรียบร้อยแล้ว เซิร์ฟเวอร์การอนุญาตจะส่งโค้ดหรือโทเค็นไปยัง URI การเปลี่ยนเส้นทาง ดังนั้นคุณจึงต้องลงทะเบียนสถานที่ที่ถูกต้องเป็นส่วนหนึ่งของกระบวนการลงทะเบียนแอป

**การเตรียมใช้งานแอปพลิเคชัน**

[บทช่วยสอน: พัฒนาและวางแผนการเตรียมใช้งาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) จุดสิ้นสุด SCIM - บทความนี้อธิบายวิธีการสร้างจุดสิ้นสุด SCIM และรวมกับบริการการเตรียมใช้งาน AAD


