---
title: ข้อผิดพลาดของแอปพลิเคชัน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931468"
---
# <a name="application-errors"></a>ข้อผิดพลาดของแอปพลิเคชัน

ค้นหาข้อมูลเกี่ยวกับรหัสข้อผิดพลาด **AADSTS ที่ส่งกลับ** จากบริการโทเค็นความปลอดภัยของ Azure Active Directory (Azure AD) (STS) อยู่ใช่หรือไม่ อ่าน [รหัสข้อผิดพลาดการรับรองความถูกต้องและการอนุญาต Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) เพื่อค้นหารายละเอียดข้อผิดพลาด AADSTS การแก้ไข และการแก้ไขปัญหาชั่วคราวที่แนะนะ

ข้อผิดพลาดในการตรวจสอบอาจเป็นผลจากปัญหาต่างๆ มากมาย โดยส่วนใหญ่จะสร้างข้อผิดพลาด 401 หรือ 403 ตัวอย่างเช่น สิ่งต่อไปนี้อาจก่อให้เกิดข้อผิดพลาดในการตรวจสอบได้ทั้งหมด:

- โฟล [ว์การรับโทเค็นการเข้าถึงที่ไม่ถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- กําหนดค่าขอบเขต [สิทธิ์ไม่ดี](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- ไม่มีความยินยอม[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

เมื่อต้องการแก้ไขข้อผิดพลาดทั่วไปในการอนุญาต ให้ลองปฏิบัติตามขั้นตอนที่ให้ไว้ด้านล่างว่าใกล้เคียงกับข้อผิดพลาดที่คุณได้รับมากที่สุด อาจมีมากกว่าหนึ่งรายการ

**ข้อผิดพลาด 401 ไม่ได้รับอนุญาต: โทเค็นของคุณถูกต้องหรือไม่**

ตรวจสอบให้แน่ใจว่าแอปพลิเคชันของคุณแสดงโทเค็นการเข้าถึงที่ถูกต้องGraph Microsoft เป็นส่วนหนึ่งของการร้องขอ ข้อผิดพลาดนี้มักจะหมายความว่าโทเค็นการเข้าถึงอาจหายไปในส่วนหัวของการร้องขอการรับรองความถูกต้อง HTTP หรือโทเค็นไม่ถูกต้องหรือหมดอายุแล้ว เราขอแนะให้ คุณใช้ไลบรารี [การรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) เพื่อการรับโทเค็นการเข้าถึง นอกจากนี้ ข้อผิดพลาดนี้อาจเกิดขึ้นถ้าคุณพยายามใช้โทเค็นการเข้าถึงที่ได้รับมอบสิทธิ์ให้กับบัญชี Microsoft ส่วนบุคคลเพื่อเข้าถึง API ที่สนับสนุนเฉพาะบัญชีที่งานหรือโรงเรียน (บัญชีขององค์กร)

**ข้อผิดพลาด 403 Forbidden: คุณได้เลือกชุดสิทธิ์ที่ถูกต้องหรือไม่**

ตรวจสอบว่าคุณได้ขอชุดสิทธิ์ที่ถูกต้องโดยยึดตาม API ของ Microsoft Graph ที่แอปของคุณเรียก สิทธิ์ที่น้อยที่สุดที่ได้รับสิทธิ์ที่แนะGraphมีอยู่ในหัวข้อวิธีการอ้างอิง API ของ Microsoft Graphทั้งหมด นอกจากนี้ สิทธิ์เหล่านั้นต้องถูกมอบให้กับแอปพลิเคชันโดยผู้ใช้หรือผู้ดูแลระบบ การให้สิทธิ์ตามปกติจะเกิดขึ้นผ่านหน้าความยินยอมหรือโดยการให้สิทธิ์โดยใช้ใบลงทะเบียนของแอปพลิเคชัน Azure Portal จาก **การตั้งค่า** Blade ของแอปพลิเคชัน **ให้คลิก สิทธิ์** ที่ต้องมี **แล้วคลิก ให้** สิทธิ์

- [สิทธิ์Graphของ Microsoft](https://docs.microsoft.com/graph/permissions-reference) 
- [การความเข้าใจสิทธิ์และความยินยอมของ Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**ข้อผิดพลาด 403 Forbidden: แอปของคุณได้รับโทเค็นเพื่อจับคู่กับสิทธิ์ที่เลือกหรือไม่**

ตรวจสอบให้แน่ใจว่าชนิดของสิทธิ์ที่ร้องขอหรือที่ได้รับตรงกับชนิดของโทเค็นการเข้าถึงที่แอปของคุณได้รับ คุณอาจร้องขอและให้สิทธิ์ของแอปพลิเคชัน แต่ใช้โทเค็นโฟลว์โค้ดแบบโต้ตอบที่ได้รับมอบสิทธิ์แทนโทเค็นโฟลว์ข้อมูลรับรองความถูกต้องของไคลเอ็นต์ หรือร้องขอและมอบสิทธิ์ที่ได้รับมอบสิทธิ์ แต่ใช้โทเค็นโฟลว์ข้อมูลรับรองไคลเอ็นต์แทนโทเค็นโฟลว์ของโค้ดที่ได้รับมอบสิทธิ์

- [เข้าถึงในนามของผู้ใช้และสิทธิ์ที่ได้รับมอบหมาย](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - โฟลว์รหัสการรับรองความถูกต้อง OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [รับสิทธิ์การเข้าถึงโดยไม่มีผู้ใช้ (บริการ daemon) และสิทธิ์ของแอปพลิเคชัน](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - โฟลว์ข้อมูลรับรองไคลเอ็นต์ OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**ข้อผิดพลาด 403 Forbidden: การตั้งค่ารหัสผ่านใหม่**

ในขณะนี้ ยังไม่มีสิทธิ์ของสิทธิ์ของแอปพลิเคชัน daemon service-to-service ที่อนุญาตการตั้งค่ารหัสผ่านผู้ใช้ใหม่ API เหล่านี้ได้รับการสนับสนุนโดยใช้โค้ดที่ได้รับมอบสิทธิ์แบบโต้ตอบกับผู้ดูแลระบบที่ลงชื่อเข้าใช้เท่านั้น

- [สิทธิ์Graphของ Microsoft](https://docs.microsoft.com/graph/permissions-reference)

**403 Forbidden: ผู้ใช้มีสิทธิ์เข้าถึงและพวกเขาได้รับสิทธิ์การใช้งานหรือไม่**

For delegated code flows, Microsoft Graph evaluates if the request is allowed based on the permissionsed to the app and the permissions that the signed-in user has. โดยทั่วไปข้อผิดพลาดนี้ระบุว่าผู้ใช้ไม่มีสิทธิ์เพียงพอที่จะร้องขอ หรือผู้ใช้ไม่ได้รับสิทธิ์การใช้งานข้อมูลที่ถูกเข้าถึง เฉพาะผู้ใช้ที่มีสิทธิ์หรือสิทธิ์การใช้งานที่ต้องใช้เท่านั้นที่สามารถร้องขอได้

**403 Forbidden: คุณเลือก API ทรัพยากรที่ถูกต้องหรือไม่**

API services like Microsoft Graph check that the aud claim (audience) in the received access token matches the value it expects for itself, and if not, it results in a 403 Forbidden error. ข้อผิดพลาดทั่วไปที่ส่งผลให้เกิดข้อผิดพลาดนี้พยายามใช้โทเค็นที่ซื้อมาให้กับ API ของ Azure AD Graph, Outlook API หรือ API SharePoint/OneDrive เพื่อเรียกใช้ Microsoft Graph (หรือในทางกลับกันด้วย) ตรวจสอบให้แน่ใจว่าทรัพยากร (หรือขอบเขต) แอปของคุณได้รับโทเค็นเพื่อให้ตรงกับ API ที่แอปนั้นเรียก

**400 การร้องขอที่ไม่ดีหรือ 403 ไม่ได้รับอนุญาต: ผู้ใช้ปฏิบัติตามนโยบายการเข้าถึงตามเงื่อนไข (CA) ขององค์กรของพวกเขาหรือไม่**

ขึ้นอยู่กับนโยบาย CA ขององค์กร ผู้ใช้ที่เข้าถึงแหล่งข้อมูล Microsoft Graph ผ่านทางแอปของคุณอาจถูกท้าทายด้วยข้อมูลเพิ่มเติมที่ไม่แสดงอยู่ในโทเค็นการเข้าถึงที่แอปของคุณได้รับตั้งแต่แรก ในกรณีนี้ แอปของคุณได้รับ 400 ที่มีข้อผิดพลาด *interaction_required* ระหว่างการรับโทเค็นการเข้าถึงหรือ 403 ที่มีข้อผิดพลาด *insufficient_claimsโทรหา* Microsoft Graph ในทั้งสองกรณี การตอบสนองข้อผิดพลาดประกอบด้วยข้อมูลเพิ่มเติมที่สามารถนําเสนอไปยังจุดสิ้นสุดอนุญาตเพื่อท้าทายผู้ใช้เพื่อดูข้อมูลเพิ่มเติม (เช่น การรับรองความถูกต้องโดยใช้หลายปัจจัยหรือการลงทะเบียนอุปกรณ์)

- [จัดการกับความท้าทายในการเข้าถึงตามเงื่อนไขโดยใช้ MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [แนวทางสําหรับนักพัฒนาสําหรับAzure Active Directoryการเข้าถึงตามเงื่อนไข](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
