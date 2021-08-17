---
title: แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO) ในองค์กร
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: c4f46306c153c8b1598329479474895ec1ac292e07f9bc61323a90d708f34885
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105547"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a>แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO) ในองค์กร

เมื่อต้องการแก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

**ฉันจะเปิดคีย์การถอดรหัส Kerberos ของบัญชีคอมพิวเตอร์ AZUREADSSO ได้อย่างไร**

เราขอแนะให้คุณสามารถทยอยคีย์การถอดรหัสของ Kerberos อย่างน้อยทุก 30 วัน เมื่อต้องการใช้วิธีนี้ด้วยตนเอง[ให้ดู วิธีการม้วนคีย์ถอดรหัส Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)

**กําหนดค่า SSO อย่างราบรื่น**

เมื่อต้องการปรับใช้ SSO อย่างราบรื่น ให้ปฏิบัติตามขั้นตอน[Azure Active Directoryลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น: การเริ่มต้นใช้งาน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)ด่วน

**การปรึกษา**

- [Azure Active Directoryการลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่น: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - ในบทความนี้ เราจะกล่าวถึงถามที่ถามบ่อยเกี่ยวกับ Azure Active Directory Seamless Single Sign-On (Seamless SSO) คอยตรวจสอบเนื้อหาใหม่ต่อไป
- [ถาม&ของ Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - บทความนี้มีข้อมูลเกี่ยวกับวิธีการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น

**แก้ไขปัญหา**

[แก้ไขปัญหาAzure Active Directoryการเข้าสู่ระบบโดยลงชื่อเข้าใช้](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)ครั้งเดียวอย่างราบรื่น - บทความนี้จะช่วยให้คุณค้นหาข้อมูลการแก้ไขปัญหาเกี่ยวกับปัญหาทั่วไปAzure Active Directory (Azure AD) การลงชื่อเข้าระบบครั้งเดียวอย่างSign-On (SSO อย่างราบรื่น)







