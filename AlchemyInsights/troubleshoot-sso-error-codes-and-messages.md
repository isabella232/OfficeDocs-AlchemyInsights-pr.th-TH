---
title: การแก้ไขปัญหารหัสข้อผิดพลาดและข้อความการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น
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
- "9367"
- "9004357"
ms.openlocfilehash: 74c783a5fb9e1388b12801fa0de92faed9e57bf14c0f99d21539e17bf1b1c284
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039013"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-error-codes-and-messages"></a>การแก้ไขปัญหารหัสข้อผิดพลาดและข้อความการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) อย่างราบรื่น

เมื่อต้องการแก้ไขรหัสข้อผิดพลาดและข้อความการเข้าสู่ระบบโดยลงชื่อเข้าใช้ครั้งเดียว (SSO) ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ตรวจสอบและแก้ไขข้อผิดพลาด SSO โดย[ไปที่รายงานกิจกรรมการลงชื่อเข้าใช้ในAzure Active Directoryพอร์ทัล](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins)
2. ดู[Azure Active Directoryการลงชื่อเข้า](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#sign-in-failure-reasons-in-the-azure-active-directory-admin-center-needs-a-premium-license)ระบบครั้งเดียวอย่างราบรื่น - บทความนี้จะช่วยให้คุณค้นหาข้อมูลการแก้ไขปัญหาเกี่ยวกับปัญหาทั่วไปAzure Active Directory (Azure AD) การลงชื่อเข้าระบบครั้งเดียวอย่าง Sign-Onราบรื่น (SSO อย่างราบรื่น)
3. ดู รหัสข้อผิดพลาดการรับรองความถูกต้องและการอนุญาต[Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information) - บทความนี้จะช่วยคุณค้นหาข้อมูลเกี่ยวกับรหัสข้อผิดพลาด AADSTS ที่ส่งกลับจากบริการโทเค็นความปลอดภัยของ Azure Active Directory (Azure AD) (STS) บทความนี้ยังช่วยให้คุณค้นหารายละเอียดข้อผิดพลาด AADSTS การแก้ไข และการแก้ไขปัญหาชั่วคราวที่แนะนว

[ถาม&ของ Microsoft](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - ดูบทความนี้เพื่อดูข้อมูลเกี่ยวกับการร้องขอฟีเจอร์หรือถามข้อสงสัยทางเทคนิคเกี่ยวกับ SSO อย่างราบรื่น

