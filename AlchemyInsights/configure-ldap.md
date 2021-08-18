---
title: กําหนดค่า LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090431"
---
# <a name="configure-ldap"></a>กําหนดค่า LDAP

เมื่อต้องการกําหนดค่า LDAP ให้ต่อไปนี้:

1. ตรวจสอบสถานภาพโดเมนของคุณบนพอร์ทัล[Azure](https://aka.ms/aadds-health)
1. ตรวจสอบให้แน่ใจว่ามีการสมัครใช้งาน Azure AD ที่ถูกต้อง และเปิดใช้งาน Azure AD Domain Services แล้ว
1. ใบรับรองที่ต้องมีเพื่อเปิดใช้งาน LDAP ที่ปลอดภัยต้องได้รับจากผู้ออกใบรับรองสาธารณะที่เชื่อถือได้หรือเป็นใบรับรองที่เซ็นชื่อด้วยตนเอง
1. ตรวจสอบให้แน่ใจว่าใบรับรองเป็นไปตามแนวทาง[ที่ต้องมี](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**ใบรับรองไม่ถูกต้อง**
1. เมื่อต้องการต่ออายุใบรับรอง ให้ปฏิบัติตามขั้นตอนเพื่อสร้างใบรับรองใหม่และโหลดใหม่:[กําหนดค่า LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. เมื่อต้องการแก้ไขปัญหาที่ทราบแล้วด้วยการแจ้งเตือน LDAP ที่ปลอดภัยใน Azure Active Directory Domain Services[ให้ดู แก้ไขการแจ้งเตือน LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
