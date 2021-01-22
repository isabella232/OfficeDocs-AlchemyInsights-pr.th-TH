---
title: ปัญหาการลงชื่อเข้าใช้ของผู้ใช้ SSO อย่างราบรื่น
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935215"
---
# <a name="seamless-sso-user-sign-in-issues"></a>ปัญหาการลงชื่อเข้าใช้ของผู้ใช้ SSO อย่างราบรื่น

หลังจากที่ผู้ใช้ได้รับการรับรองความถูกต้องแล้ว เบราว์เซอร์จะแคชข้อมูลรับรองความถูกต้องของผู้ใช้ เพื่อให้ในเบราว์เซอร์เดียวกัน แอปพลิเคชันจะลงชื่อเข้าใช้ด้วยบัญชีเดียวกันโดยอัตโนมัติ ซึ่งอาจสร้างความยุ่งยากให้ผู้ใช้อื่นหรือผู้ใช้รายเดียวเข้าสู่ระบบหลายบัญชีในอุปกรณ์หนึ่งเครื่อง เมื่อต้องการแก้ไขปัญหานี้: 1. ลองลงชื่อเข้าใช้บนเบราว์เซอร์อื่น 2. ล้างแคชและ/หรือคุกกี้ของเบราว์เซอร์ แล้วลองลงชื่อเข้าใช้อีกครั้ง

ถ้าคุณยังคงพบปัญหาในการลงชื่อเข้าใช้ เราขอแนะนนะต่อไปนี้เพื่อวินิจฉัยและปฏิบัติตามขั้นตอนการแก้ปัญหาโดยอัตโนมัติ:

1. ติดตั้งโปรแกรม [เสริมเบราว์เซอร์ที่ปลอดภัยของแอป](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) ของฉันเพื่อช่วยให้ Azure Active Directory (Azure AD) แสดงการใช้งานและการแก้ไขปัญหาที่ดียิ่งขึ้นเมื่อใช้ประสบการณ์การทดสอบในพอร์ทัล Azure
2. เกิดข้อผิดพลาดเกิดข้อผิดพลาดโดยใช้ประสบการณ์การทดสอบในหน้าการกําหนดค่าแอปในพอร์ทัล Azure เมื่อต้องการเรียนรู้เพิ่มเติม ดู[แอปพลิเคชันการลงชื่อเข้าระบบครั้งเดียวที่ใช้ DEBUG SAML](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)
3. ถ้าคุณใช้ประสบการณ์การทดสอบในพอร์ทัล Azure ด้วยโปรแกรมเสริมเบราว์เซอร์ที่ปลอดภัยของแอปของฉัน คุณสามารถข้ามขั้นตอนที่ **4**
4. เมื่อต้องการเปิดหน้าการกําหนดค่าการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวที่ใช้ SAML:
    - เปิด [พอร์ทัล Azure](https://portal.azure.com/)และลงชื่อเข้าใช้ในฐานะ **ผู้ดูแลระบบส่วนกลาง** หรือ **Coadmin**
    - เปิดส่วนขยาย **Azure Active Directory** โดยการเลือก **บริการ** ทั้งหมดที่ด้านบนของเมนูการนําทางด้านซ้ายหลัก
    - พิมพ์ "Azure Active Directory" ในกล่องค้นหาตัวกรอง แล้วเลือก **รายการ Azure Active Directory**
    - เลือก **แอปพลิเคชันองค์กร** จากเมนูการนําทางด้านซ้ายของ Azure Active Directory
    - **เลือก แอปพลิเคชัน** ทั้งหมด เพื่อดูรายการแอปพลิเคชันของคุณทั้งหมด ถ้าคุณไม่เห็นแอปพลิเคชันที่คุณต้องการแสดงอยู่ที่นี่ ให้ใช้ตัวควบคุม ตัวกรอง ที่ด้านบนของ รายการแอปพลิเคชันทั้งหมด และตั้งค่าตัวเลือก **แสดง** เป็น **แอปพลิเคชัน** ทั้งหมด
    - เลือกแอปพลิเคชันที่คุณต้องการกําหนดค่าให้ลงชื่อเข้าใช้ครั้งเดียว
    - หลังจากโหลดแอปพลิเคชันแล้ว **ให้เลือกการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว** จากเมนูการนําทางด้านซ้ายของแอปพลิเคชัน
    - เลือก **SSO แบบใช้ SAML**
5. โดยยึดตามข้อผิดพลาด เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับขั้นตอนที่แนะนําให้ปฏิบัติตาม ให้ดูที่ ปัญหาในการลงชื่อเข้าใช้แอปที่กําหนดค่าการลงชื่อเข้าระบบครั้งเดียว[ที่ใช้ SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. เมื่อต้องการแก้ไขปัญหาการเข้าสู่ระบบของผู้ใช้อื่น ให้ดูคู่มือต่อไปนี้:
    - [โพรโทคอลSign-On SAML แบบใช้ครั้งเดียว](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [วิธีการ: แก้ไขปัญหาข้อผิดพลาดในการเข้าสู่ระบบโดยใช้รายงาน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [พร้อมท์ความยินยอมที่ไม่คาดคิด](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [ข้อผิดพลาดการยินยอมจากผู้ใช้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [ปัญหาในการลงชื่อเข้าใช้จากแอปของฉัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [ข้อผิดพลาดบนหน้าลงชื่อเข้าใช้แอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [ปัญหาในการลงชื่อเข้าใช้แอป Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
