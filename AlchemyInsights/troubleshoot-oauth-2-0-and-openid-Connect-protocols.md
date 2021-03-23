---
title: แก้ไขปัญหาโพรโทคอล OAuth 2.0 และ OpenID Connect
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
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037696"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>แก้ไขปัญหาโพรโทคอล OAuth 2.0 และ OpenID Connect

เมื่อต้องการแก้ไขปัญหา OAuth 2.0 และ OpenID Connect ให้ปฏิบัติตามขั้นตอนที่แนะนาต่อไปนี้:

ดูบทความต่อไปนี้ที่เกี่ยวข้องกับการกําหนดค่าและการแก้ไขปัญหาโพรโทคอล OAuth 2.0 และ OpenID Connect:

- แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft และโฟลว์รหัสการรับรองความถูกต้อง [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - บทความนี้อธิบายวิธีการเขียนโปรแกรมกับโฟลว์การให้รหัส **(PKCE)** โดยตรงในแอปพลิเคชันของคุณ โดยใช้ภาษาใดก็ได้
- [แพลตฟอร์มข้อมูลเฉพาะตัวของไมโครซอฟท์และข้อมูลเฉพาะตัวของไคลเอ็นต์ OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟลว์ข้อมูล **เฉพาะตัวของไคลเอ็นต์** ในแอปพลิเคชันของคุณ
- [แพลตฟอร์มข้อมูลเฉพาะตัวของไมโครซอฟท์และข้อมูลเฉพาะตัวของรหัสผ่านเจ้าของทรัพยากร OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟล **ว์ ROPC** ในแอปพลิเคชันของคุณ
    - แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft สนับสนุนเฉพาะ ROPC ของผู้เช่า Azure AD เท่านั้น และไม่รองรับบัญชีส่วนบุคคล ซึ่งหมายความว่าคุณต้องใช้จุดสิ้นสุดเฉพาะผู้เช่า **( https://login.microsoftonline.com/{TenantId_or_Name})****หรือจุดสิ้นสุด** องค์กร)
    - บัญชีส่วนบุคคลที่ได้รับเชิญให้เข้าร่วมผู้เช่า Azure AD จะใช้งาน ROPC ไม่ได้
    - บัญชีที่ไม่มีรหัสผ่านไม่สามารถลงชื่อเข้าใช้ผ่าน ROPC ในสถานการณ์สมมตินี้ เราขอแนะนนะให้คุณใช้โฟลว์ที่แตกต่างกันในแอปของคุณแทน
    - ถ้าผู้ใช้ต้องใช้ [การรับรองความถูกต้องโดยใช้หลายปัจจัย (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) เพื่อเข้าสู่ระบบแอปพลิเคชัน พวกเขาจะถูกบล็อก
    - ROPC ไม่ได้รับการสนับสนุนในสถานการณ์ [การติดต่อกับภายนอก](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) ข้อมูลเฉพาะตัวแบบไฮบริด (ตัวอย่างเช่น Azure AD และ ADFS ที่ใช้เพื่อรับรองความถูกต้องของบัญชีภายในองค์กร) ถ้าผู้ใช้เปลี่ยนเส้นทางแบบเต็มหน้าไปยังผู้ให้บริการข้อมูลเฉพาะตัวภายในองค์กร Azure AD จะไม่สามารถทดสอบชื่อผู้ใช้และรหัสผ่านกับผู้ให้บริการข้อมูลเฉพาะตัวนั้น [อย่างไรก็ตาม การรับรองความถูกต้องแบบ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) พาส-ผ่านได้รับการสนับสนุนกับ ROPC
    - ข้อยกเว้นของสถานการณ์การติดต่อกับภายนอกของข้อมูลเอกลักษณ์แบบไฮบริดจะเป็นดังต่อไปนี้: นโยบาย Home Realm Discovery ที่มี **การตั้งค่า AllowCloudPasswordValidation** **เป็น TRUE** จะเปิดใช้งานโฟลว์ ROPC เพื่อใช้งานกับผู้ใช้ภายนอกเมื่อซิงค์รหัสผ่านภายในองค์กรกับระบบคลาวด์ For more information, see [Enable direct ROPC authentication of federrated users for legacy applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft และ [OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - บทความนี้อธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟลว์ **ในนามของ (OBO)** ในแอปพลิเคชันของคุณ
- [แพลตฟอร์มข้อมูลเฉพาะตัวของไมโครซอฟท์](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) และโพรโทคอล OpenID Connect - บทความนี้แสดงวิธีการใช้โพรโทคอล OpenID Connect ที่ไม่ขึ้นกับภาษา และอธิบายวิธีการส่งและรับข้อความ HTTP โดยไม่ต้องใช้ไลบรารีโอเพนซอร์สใดๆ ของ Microsoft

**เข้าถึงโทเค็น**

[โทเค็นการเข้าถึงแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - เรียนรู้วิธีที่ API ของคุณสามารถตรวจสอบและใช้การอ้างสิทธิ์ภายในโทเค็นการเข้าถึง เอกสารประกอบทั้งหมดในบทความนี้ ยกเว้นที่บันทึกที่บันทึกจะใช้ได้กับโทเค็นที่ออกให้กับ API ที่คุณได้ลงทะเบียนเท่านั้น ไม่สามารถใช้กับโทเค็นที่ออกให้กับ API ที่ Microsoft เป็นเจ้าของ หรือสามารถใช้โทเค็นเหล่านั้นเพื่อตรวจสอบวิธีที่แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft จะออกโทเค็นให้กับ API ที่คุณสร้าง

**การกําหนดค่าแอปพลิเคชัน**

[การเปลี่ยนเส้นทางข้อจํากัดและข้อจํากัด URI (URL](https://docs.microsoft.com/azure/active-directory/develop/reply-url) ตอบกลับ) - เรียนรู้วิธีกําหนดค่า URI การเปลี่ยนเส้นทาง (URL ตอบกลับ) ของคุณ การเปลี่ยนเส้นทาง URI หรือ URL ตอบกลับ คือสถานที่ที่เซิร์ฟเวอร์การอนุญาตส่งผู้ใช้เมื่อแอปได้รับการอนุมัติแล้ว และให้รหัสการตรวจสอบหรือโทเค็นการเข้าถึง เซิร์ฟเวอร์การรับรองความถูกต้องจะส่งโค้ดหรือโทเค็นไปยัง URI การเปลี่ยนเส้นทาง ดังนั้นคุณจึงต้องลงทะเบียนสถานที่ที่ถูกต้องให้เป็นส่วนหนึ่งของกระบวนการลงทะเบียนแอป

**การเตรียมใช้งานแอปพลิเคชัน**

[บทช่วยสอน: พัฒนาและวางแผนการเตรียมใช้งาน](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) จุดสิ้นสุด SCIM - บทความนี้อธิบายวิธีการสร้างจุดสิ้นสุด SCIM และรวมกับบริการการเตรียมใช้งาน AAD


