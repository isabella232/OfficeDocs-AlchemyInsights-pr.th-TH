---
title: แก้ไขปัญหาการรับรองความถูกต้อง SSO แบบใช้ SAML
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "9409"
ms.openlocfilehash: c053e252edfcc51c95214c4bff4aded2bded2e23
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695665"
---
# <a name="troubleshoot-saml-based-sso-authentication-issues"></a>แก้ไขปัญหาการรับรองความถูกต้อง SSO แบบใช้ SAML

ผู้ใช้ส่วนใหญ่สามารถแก้ไขปัญหาการรับรองความถูกต้อง SSO แบบ SAML โดยใช้ขั้นตอนที่แนะนําต่อไปนี้:

**ขั้นตอนที่แนะนา**
1. ค้นหา [ข้อมูลรหัสข้อผิดพลาด](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#lookup-current-error-code-information)ปัจจุบัน
1. ดู [การลงชื่อเข้าระบบครั้งเดียวโดยใช้ DEBUG SAML ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/debug-saml-sso-issues) เพื่อแก้ไขข้อผิดพลาดการรับรองความถูกต้อง
1. ดูบทความ โพรโทคอล [SAML Sign-On เดี่ยว](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol) เพื่อเรียนรู้เกี่ยวกับการร้องขอการรับรองความถูกต้อง SAML 2.0 และการตอบกลับที่ Azure Active Directory (Azure AD) สนับสนุน Sign-On เดี่ยว (SSO)


