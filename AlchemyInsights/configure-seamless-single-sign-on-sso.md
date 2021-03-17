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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841670"
---
# <a name="configure-seamless-single-sign-on-sso"></a>กําหนดค่าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO)

**กําหนดค่าแอปพลิเคชัน**

1. คุณควรได้รับค่าจากผู้ออกแอปพลิเคชัน คุณสามารถใส่ค่าหรืออัปโหลดไฟล์ Metadata ด้วยตนเองเพื่อแยกค่าของเขตข้อมูล
2. แอปมากมายได้รับการกําหนดค่าไว้ล่วงหน้าให้ใช้งานกับ Azure AD แอปเหล่านี้จะแสดงอยู่ในแกลเลอรีแอปที่คุณสามารถเรียกดูได้เมื่อคุณเพิ่มแอปลงในผู้เช่า Azure AD ของคุณ ชุด [คู่มือการเริ่มต้นใช้งานฉบับด่วน](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) จะช่วยให้คุณสามารถอ่านขั้นตอนต่างๆ ได้
3. เมื่อต้องการสร้างแอปพลิเคชันที่ไม่ใช่แกลเลอรี คุณสามารถคลิกที่ปุ่ม **+ สร้างแอปพลิเคชัน** ของคุณเอง และตั้งชื่อแอปพลิเคชันของคุณ
    - ตามค่าเริ่มต้น แอปจะเลือก **รวมแอปพลิเคชันอื่นๆ ที่คุณไม่พบในแกลเลอรี** ซึ่งเป็นตัวเลือกที่ถูกต้องของแอปพลิเคชันที่ไม่ใช่แกลเลอรี
    - เมื่อคุณกด **สร้าง** หลังจากใส่ชื่อแอปพลิเคชัน แอปจะสร้างแอปพลิเคชัน Enterprise แบบ Non-gallery ใหม่
    - จากนั้น คุณสามารถนําทาง **ไปยังการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว** ภายใต้จัดการแอปพลิเคชันนั้น และคุณจะสามารถดูเทคนิคต่างๆ เพื่อปรับใช้ในสภาพแวดล้อมของคุณ

**กําหนดค่า SSO อย่างราบรื่นในแอปพลิเคชันเฉพาะ**

ส่วนแอปในแกลเลอรีคุณจะพบคําแนะนําโดยละเอียดทีละขั้นตอน เมื่อต้องการเข้าถึงขั้นตอนคุณสามารถเรียกดูรายการของบทช่วยสอนการกําหนดค่าแอปทั้งหมดที่บทช่วย[สอนการกําหนดค่าแอป SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**การกําหนดค่า SSO แบบใช้ SAML**

1. [การเริ่มต้นใช้งานด่วน: ตั้งค่าการลงชื่อเข้าระบบครั้งเดียวแบบ SAML (SSO) ของแอปพลิเคชันในผู้เช่า Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)ของคุณ
2. เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับตัวเลือกที่ใช้ SAML ในการลงชื่อเข้าระบบครั้งเดียว ให้ดูที่ เข้าใจการลงชื่อเข้า[ระบบครั้งเดียวที่ใช้ SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. เมื่อต้องการเรียนรู้เกี่ยวกับการร้องขอและการตอบกลับการรับรองความถูกต้อง SAML 2.0 ที่ Azure Active Directory (Azure AD) สนับสนุน Single Sign-On (SSO) ให้ดูโพรโทคอล [SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)Sign-On เดี่ยว
4. เมื่อต้องการเรียนรู้วิธีการสร้างและกําหนดค่าการลงชื่อเข้าระบบครั้งเดียว (SSO) แบบ SAML ของแอปพลิเคชันใน Azure Active Directory (Azure AD) โดยใช้ Microsoft Graph API ให้ดู การกําหนดค่าการลงชื่อเข้าระบบครั้งเดียวแบบ [SAML](https://docs.microsoft.com/graph/application-saml-sso-configure-api)ของแอปพลิเคชันของคุณโดยใช้ Microsoft Graph API
5. เมื่อต้องการเรียนรู้วิธีที่ Azure AD ใช้โพรโทคอล SAML[ให้ดูวิธีการใช้แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft ที่ใช้โพรโทคอล SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**กําหนดค่าโทเค็นและการอ้างสิทธิ์**

1. [วิธีการ: ปรับแต่งการอ้างสิทธิ์ที่ออกในโทเค็น SAML ของแอปพลิเคชันระดับ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)องค์กร
2. To learn how to configure claims using PowerShell, see [How to: Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. เมื่อต้องการเรียนรู้วิธีการกําหนดค่าการอ้างสิทธิ์เพิ่มเติม ให้ดู [วิธีการ: ให้การอ้างสิทธิ์เพิ่มเติมกับแอป](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)ของคุณ
4. To learn how to use directory schema extension attributes for sending user data to applications in token claims, [see Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. เมื่อต้องการเรียนรู้วิธีการกําหนดอายุการใช้งานโทเค็น ให้ดูอายุการใช้งานโทเค็นที่กําหนด[ค่าได้ในแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft (ตัวอย่าง)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [กําหนดค่านโยบายอายุการใช้งานโทเค็น (ตัวอย่าง)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - ในบทความนี้ เราจะปฏิบัติตามสถานการณ์สมมติของนโยบายทั่วไปที่สามารถช่วยให้คุณกําหนดกฎใหม่อายุการใช้งานโทเค็นได้ ในตัวอย่าง คุณเรียนรู้วิธีสร้างนโยบายที่ให้ผู้ใช้ต้องรับรองความถูกต้องบ่อยครั้งขึ้นในเว็บแอปของคุณ

**แก้ไขปัญหาการกําหนดค่า SSO**

- For frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO), see [Azure Active Directory seamless single sign-on: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- ดูข้อมูลการแก้ไขปัญหาทั่วไปเกี่ยวกับ Azure Active Directory (Azure AD) การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นSign-On (SSO อย่างราบรื่น) ดูการแก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นของ[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
