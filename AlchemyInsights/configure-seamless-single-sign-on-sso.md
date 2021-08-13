---
title: กําหนดค่าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966056"
---
# <a name="configure-seamless-single-sign-on-sso"></a>กําหนดค่าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO)

**กําหนดค่าแอปพลิเคชัน**

1. คุณควรได้รับค่าจากผู้ขายแอปพลิเคชัน คุณสามารถใส่ค่าหรืออัปโหลดไฟล์เมตาดาต้าด้วยตนเองเพื่อแยกค่าของเขตข้อมูลได้
2. หลายแอปได้รับการกําหนดค่าล่วงหน้าให้ใช้งานกับ Azure AD อยู่แล้ว แอปเหล่านี้จะแสดงอยู่ในแกลเลอรีแอปที่คุณสามารถเรียกดูได้เมื่อคุณเพิ่มแอปลงในผู้เช่า Azure AD ของคุณ ชุด [การเริ่มต้นใช้งานด่วน](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) จะช่วยให้คุณสามารถดูกระบวนการต่างๆ ได้
3. เมื่อต้องการสร้างแอปพลิเคชันที่ไม่ใช่แกลเลอรี คุณสามารถคลิกปุ่ม **+ สร้างแอปพลิเคชัน** ของคุณเอง แล้วตั้งชื่อแอปพลิเคชันของคุณ
    - ตามค่าเริ่มต้น จะเลือก **รวมแอปพลิเคชันอื่นๆ ที่คุณไม่พบในแกลเลอรี** ซึ่งเป็นตัวเลือกที่ถูกต้องของแอปพลิเคชันที่ไม่ใช่แกลเลอรี
    - เมื่อคุณกด **สร้าง** หลังจากใส่ชื่อของแอปพลิเคชัน แอปจะสร้างแอปพลิเคชันองค์กรที่ไม่มีแกลเลอรีใหม่
    - จากนั้น คุณอาจนําทาง **ไปยัง การ** ลงชื่อเข้าระบบครั้งเดียว ภายใต้ จัดการแอปพลิเคชันนั้น และคุณจะสามารถดูเทคนิคต่างๆ เพื่อนําไปปรับใช้ในสภาพแวดล้อมของคุณ

**กําหนดค่า SSO อย่างราบรื่นของแอปพลิเคชันเฉพาะ**

For the apps in the gallery you will find detailed, step-by-step, instructions. เมื่อต้องการเข้าถึงขั้นตอน คุณสามารถเรียกดูรายการของบทช่วยสอนการกําหนดค่าแอปทั้งหมดที่[บทช่วยสอนการกําหนดค่าแอป SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**การกําหนดค่า SSO แบบใช้ SAML**

1. [การเริ่มต้นใช้งานด่วน: ตั้งค่าการลงชื่อเข้าระบบครั้งเดียว (SSO) แบบ SAML ของแอปพลิเคชันในผู้เช่า Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)ของคุณ
2. เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับตัวเลือกที่ใช้ SAML ในการลงชื่อเข้าระบบครั้งเดียว ให้ดูที่ [การลงชื่อเข้าระบบ](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)ครั้งเดียวแบบ SAML
3. เมื่อต้องการเรียนรู้เกี่ยวกับการร้องขอการรับรองความถูกต้อง SAML 2.0 และการตอบกลับAzure Active Directory (Azure AD) ที่สนับสนุน Single Sign-On (SSO) ให้ดูที่ โพรโทคอล[SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)Sign-Onเดี่ยว
4. เมื่อต้องการเรียนรู้วิธีการสร้างและกําหนดค่าการลงชื่อเข้าระบบครั้งเดียว (SSO) แบบ SAML ของแอปพลิเคชันใน Azure Active Directory (Azure AD) โดยใช้ Microsoft Graph API ให้ดู การกําหนดค่าการลงชื่อเข้าระบบครั้งเดียวแบบ[SAML](https://docs.microsoft.com/graph/application-saml-sso-configure-api)ของแอปพลิเคชันของคุณโดยใช้ Microsoft Graph API
5. เมื่อต้องการเรียนรู้วิธีใช้โพรโทคอล SAML ของ Azure AD[ให้ดู วิธีที่แพลตฟอร์มข้อมูลประจําตัวของ Microsoftใช้โพรโทคอล SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**กําหนดค่าโทเค็นและการอ้างสิทธิ์**

1. [วิธีการ: ปรับแต่งการอ้างสิทธิ์ที่ออกในโทเค็น SAML For Enterprise](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)Applications
2. To learn how to configure claims using PowerShell, [see How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. เมื่อต้องการเรียนรู้วิธีการกําหนดค่าการอ้างสิทธิ์เพิ่มเติม [ให้ดู วิธีการ: ให้การอ้างสิทธิ์เพิ่มเติมกับแอป](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)ของคุณ
4. To learn how to use directory schema extension attributes for sending user data to applications in token claims, [see Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. เมื่อต้องการเรียนรู้วิธีการกําหนดอายุการใช้งานโทเค็น ให้ดู อายุการใช้งาน[โทเค็นที่กําหนดค่าได้แพลตฟอร์มข้อมูลประจําตัวของ Microsoft (ตัวอย่าง)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [กําหนดค่านโยบายอายุการใช้งานโทเค็น (ตัวอย่าง)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - ในบทความนี้ เราจะปฏิบัติตามสถานการณ์นโยบายทั่วไปที่สามารถช่วยให้คุณกําหนดกฎใหม่อายุการใช้งานโทเค็น ในตัวอย่าง คุณจะได้เรียนรู้วิธีการสร้างนโยบายที่ต้องการให้ผู้ใช้รับรองความถูกต้องได้บ่อยขึ้นในเว็บแอปของคุณ

**แก้ไขปัญหาการกําหนดค่า SSO**

- For frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO), see [Azure Active Directory Seamless Single Sign-on: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- For troubleshooting information about common problems about Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO), see [Troubleshoot Azure Active Directory Seamless Single Sign-on](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).
