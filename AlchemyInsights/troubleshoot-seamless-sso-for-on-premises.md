---
title: แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO) ภายในองค์กร
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
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816347"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a>แก้ไขปัญหาการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียวอย่างราบรื่น (SSO) ภายในองค์กร

เมื่อต้องการแก้ไขปัญหาการลงชื่อเข้าระบบครั้งเดียว (SSO) อย่างราบรื่น ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

**ฉันจะเปิดคีย์การถอดรหัส Kerberos ของบัญชีคอมพิวเตอร์ AZUREADSSO ได้อย่างไร**

เราขอแนะนนะให้คุณใช้คีย์การถอดรหัส Kerberos อย่างน้อยทุก 30 วัน To do this manually, [see how to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).

**กําหนดค่า SSO อย่างราบรื่น**

เมื่อต้องการปรับใช้ SSO อย่างราบรื่น ให้ปฏิบัติตามขั้นตอนในการลงชื่อเข้าระบบครั้งเดียว [อย่างราบรื่นของ Azure Active Directory: การเริ่มต้นใช้งาน](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)ด่วน

**ที่ปรึกษา**

- การลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นของ[Azure Active Directory: Frequently asked](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) questions - ในบทความนี้ เราจะตอบถามที่ถามบ่อยเกี่ยวกับ Azure Active Directory Seamless Single Sign-On (Seamless SSO) คอยตรวจสอบเนื้อหาใหม่อยู่
- [ถามตอบ&ของ Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - บทความนี้มีข้อมูลเกี่ยวกับวิธีการสร้างการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น

**แก้ไขปัญหา**

[แก้ไขปัญหาการ](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) ลงชื่อเข้าระบบครั้งเดียวอย่างราบรื่นของ Azure Active Directory - บทความนี้ช่วยให้คุณค้นหาข้อมูลการแก้ไขปัญหาทั่วไปเกี่ยวกับ Azure Active Directory (Azure AD Sign-On) การเข้าสู่ระบบครั้งเดียวอย่างราบรื่น (SSO อย่างราบรื่น)







